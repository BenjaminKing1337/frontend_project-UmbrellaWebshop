<template>
    <div class="delete">
        <AdminNav/>
        <div class="content">
            <div class="sheet">
                <li>ID: <input v-model="id" type="number"></li>
            </div>
            <div class="footer"><h1 v-on:click="save">GO</h1></div>
        </div>

    </div>
</template>

<script>
    import restApi from '../../api/api'
    import AdminNav from './AdminNav.vue'
    export default {
        name: "Delete",
        components: {
            AdminNav
        },
        data () {
            return {
                id: 1,
            }
        },
        methods: {
            save() {
                const baseURI = 'https://umbrellashopuirestapi20191009103803.azurewebsites.net/api/umbrella/'
                restApi.delete(baseURI + this.id)
                    .then((result) => {
                        // eslint-disable-next-line no-console
                        console.log(result);
                    })
            }
        }
    }
</script>

<style scoped>
    .delete{
        display: flex;
        width: 100%;
        height: 100%;
    }
    .content{
        padding-top: 100px;
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
    }
    .footer{
        color: white;
        width: 100%;
        height: 100px;
        background: purple;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .sheet{
        font-size: 50px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-around;
        background: white;
        height: 50%;
        width: 50%;
        border: 2px black solid;
    }
    .sheet input {
        background: rgba(255, 28, 57, 0.39);
    }
</style>
<template>
    <div class="post">
        <AdminNav/>
        <div class="content">
            <div class="sheet">
                    <li>Brand: <input v-model="brand" type="text" name="fname"></li>
                    <li>Type: <input v-model="type" type="text" name="fname"></li>
                    <li>Color: <input v-model="color" type="text" name="fname"></li>
                    <li>Size: <input v-model="size" type="number" name="fname"></li>
                    <li>Price: <input v-model="price" type="number" name="fname"></li>
            </div>
            <div class="footer">
                <h1 v-on:click="save">GO</h1>
            </div>
        </div>

    </div>
</template>

<script>
    import restApi from '../../api/api'
    import AdminNav from './AdminNav.vue'
    export default {
        name: "Post",
        components: {
            AdminNav
        },
        data () {
            return {
                brand: '',
                type: '',
                color: '',
                size: 1,
                price: 69,
            }
        },
        methods: {
            save() {
                const baseURI = 'https://umbrellashopuirestapi20191009103803.azurewebsites.net/api/umbrella'
                restApi.post(baseURI, {
                    brand: this.brand,
                    type: this.type,
                    color: this.color,
                    size: this.size,
                    price: this.price
                })
                    .then((result) => {
                        // eslint-disable-next-line no-console
                        console.log(result);
                    })
            }
        }
    }
</script>

<style scoped>
    .post{
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
        font-size: 30px;
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
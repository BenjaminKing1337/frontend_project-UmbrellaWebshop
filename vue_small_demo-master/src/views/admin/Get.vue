<template>
    <div id="get">
        <AdminNav/>
        <div class="content">
            <div>
            <div class="types">
            <select v-on:click="fetchAlbums(selected)" v-model="selected">
                <option disabled value="">Please select one</option>
                <option>Umbrella</option>
                <option>Order</option>
                <option>Customer</option>
            </select>
        </div>


            <div class="card_container">
                    <v-card
                            v-for="umbrella in umbrellas"
                            v-bind:key="umbrella.productId"
                            max-width="344"

                    >
                        <v-card-text>{{umbrella}}</v-card-text>
                    </v-card>
            </div>
            </div>
        </div>


    </div>
</template>

<script>
    import restApi from '../../api/api'
    import AdminNav from './AdminNav.vue'
    export default {
        name: "Get",
        components: {
            AdminNav
        },
        mounted(){
            this.fetchAlbums(this.selected);
        },
        data () {
            return {
                selected: 'Umbrella',
                umbrellas: [],
                deletedSuccess: false,
                deletedText: 'Album deleted'
            }
        },
        methods: {
            fetchAlbums(type) {
                restApi.get(type)
                    .then((result) => {
                        if (this.umbrellas && this.umbrellas.length > 0){
                            this.umbrellas = null;
                        }
                        this.umbrellas = result.data
                    })
            },
    }
    }
</script>

<style scoped>
    select{
        background: #d9e0e7;
        padding: 5px;
        font-size: 20px;
    }
    #get{

        height: 100%;
        display: flex;



    }
    .card_container{
        display: flex;
        justify-content: space-around;
        align-items: center;
        width: 60vw;
        flex-wrap: wrap;
    }

    .v-card.v-sheet.theme--light {
        margin: 10px;

    }
    .listing{
        color: #000000;
        background-color: #d9e0e7;
        width: 80%;
        border: 2px black solid;
        padding: 10px;
    }
    .content{
        padding: 20px;
        width: 85%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
    }

</style>
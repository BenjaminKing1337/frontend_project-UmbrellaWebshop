<template>
    <div class = "admin">
            <div class="nav">
                <div class="nav_list">
                    <ul>
                        <router-link to="/admin/get" class="routerLink"><li><a>Get</a></li></router-link>
                        <router-link to="/admin/post" class="routerLink"><li><a>Post</a></li></router-link>
                            <router-link to="/admin/put" class="routerLink"><li><a>Put</a></li></router-link>
                                <router-link to="/admin/delete" class="routerLink"><li><a>Delete</a></li></router-link>
                    </ul>
                </div>
            </div>
    </div>
</template>

<script>
    import restApi from '../../api/api'
    export default {
            name: "AdminNav",
                async deleteAlbum(album) {
                    let result = await restApi.delete('albums/'+album.id)
                    this.deletedSuccess = true;
                    if(result.status !== 200) {
                        // this.albums.push(album)
                    } else {
                        this.fetchAlbums()
                    }

                }
        };
</script>

<style scoped>

    .admin{
        display: flex;
        width: 15%;
        min-height: 100vh;
    }

    .nav{
        display: flex;
        background: #2c3e50;
        height: auto;
        flex-wrap: wrap;
        width: 100%;
    }

    .content li{
        font-size: 15px;
        color: #959da4;
        align-items: center;
        height: 50px;
        display: flex;
        width: 500px;
    }
    .nav_list{
        height: 50%;
    }
    .types{
        height: 50%;
        width: 200px;
        background: white;
        padding: 10px;
    }
    .nav_list li{
        font-size: 30px;
        color: #959da4;
        align-items: center;
        justify-content: center;
        height: 70px;
        display: flex;
        width: 15vw;
    }
    .nav_list li:hover{
        background: white;
        color: black;
    }

</style>
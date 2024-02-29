<script>

    export default {

        name: 'AppNav',
        
        data() {
            return {
                navLinks:[

                    'CAHARACTERS',
                    'COMICS',
                    'MOVIE',
                    'TV',
                    'GAMES',
                    'COLLECTIBLES',
                    'VIDEO',
                    'FANS',
                    'NEWS',
                    'SHOP',

                ]
                    
                
            }
        }
    }


</script>

<template>

    <div class="nav">

        <div class="nav-container">
            <div class="logo">
                <img src="../../public/dc-logo.png" alt="#">
            </div>
            <div class="list">
                <ul>
                    <li v-for="currentLink in navLinks">{{currentLink}}</li>
                </ul>
            </div>
        </div>

    </div>

</template>

<style lang="scss">

@use '../../src/style/variables' as *;



.nav{

    display: flex;
    justify-content: center;
    align-items: center;

    background-color: white;

    width: 100%;

    padding: 20px 0;

    .nav-container{

        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;

        width: 80%;

        .logo{

            height: 80px;
            width: 80px;

            img{

                height: 100%;
                width: 100%;

            }

        }

        .list{

            height: 100%;
            
            ul{
                display: flex;
                flex-wrap: wrap;
                gap: 35px;
            
                list-style-type: none;

                color: black;

                li{

                    border-bottom: 5px solid $primarycolor;

                }
            }

        }

    }

}

</style>

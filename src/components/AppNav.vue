<script>

    export default {

        name: 'AppNav',

    }

</script>

<template>

    <div class="nav">

        <div class="nav-container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="#">
            </div>
            <div class="list">
                <ul>
                    <li>CHARACTERS</li>
                    <li>COMICS</li>
                    <li>MOVIE</li>
                    <li>TV</li>
                    <li>GAMES</li>
                    <li>COLLECTIBLES</li>
                    <li>VIDEO</li>
                    <li>FANS</li>
                    <li>NEWS</li>
                    <li>SHOP</li>
                </ul>
            </div>
        </div>

    </div>

</template>

<style>

.nav{

    display: flex;
    justify-content: center;
    align-items: center;

    background-color: white;

    width: 100%;

    padding: 20px 0;

.nav-container{

    display: flex;
    justify-content: space-around;
    align-items: center;

    width: 100%;

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
            gap: 35px;
        
            list-style-type: none;

            color: black;

            li{

                border-bottom: 5px solid #0c7cec;

            }
        }

    }

}

}

</style>

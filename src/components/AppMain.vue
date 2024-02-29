<script>

    import AppMerch from '../components/AppMerch.vue';

    export default {

        name: 'AppMain',
        components: {AppMerch}

    }

</script>

<template>

    <div class="main">
        <div class="main-content">
            <div class="link">
                <a href="#"> &rightarrow;   Content goes here   &leftarrow; </a>
            </div>
        </div>
        <AppMerch></AppMerch>
        

    </div>

</template>

<style>

.main{

    display: flex;
    align-items: center;
    flex-direction: column;

    .main-content{

        display: flex;
        justify-content: center;
        align-items: center;

        width: 100%;

        background-color: black;

        .link{

            width: 80%;

            padding: 50px 0;

            a{

                color: white;
                text-decoration: none;

                font-size: 30px;

            }

        }

    }


}

</style>

<script>

    export default {

        name: 'AppComics',

        props: {
            comicsThumb: String,
            comicsSeries: String,
        },

        data() {
        },

    }

</script>

<template>

    <div class="comics">
        <div class="img-box">
            <img :src="comicsThumb" alt="#">        
        </div>
        <div class="text">
            <h4>{{ comicsSeries }}</h4>
        </div>
    </div>

</template>

<style>

.comics{
    width: calc(100% / 6 - 20px / 6 * 5);

    margin-bottom: 25px;

    .img-box{

        height: 190px;
        width: 100%;

        display: flex;
        justify-content: center;

        margin-bottom: 10px;
        
        img{
            height: 190px;
            width: 190px;
    
            object-fit: cover;
            object-position: top;
    
        }
    }

    .text{
        width: 100%;
        display: flex;
        justify-content: center;

        h4{
            width: 190px;
        }
    }
}

</style>
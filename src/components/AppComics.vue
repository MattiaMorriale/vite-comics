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
        <img :src="comicsThumb" alt="#">        
        <h4>{{ comicsSeries }}</h4>
    </div>

</template>

<style>

.comics{
    width: calc(100% / 6 - 20px / 6 * 5);

    margin-bottom: 25px;
    

    img{
        height: 190px;
        width: 190px;

        object-fit: cover;
        object-position: top;

        margin-bottom: 10px;
    }
    

}

</style>
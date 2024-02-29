<script>

    export default {

        name: 'AppMerch',

        data() {
            return {
                
                links:[

                    {
                        img:'../../public/buy-comics-digital-comics.png',
                        name:'DIGITALS COMICS',
                    },
                    {
                        img:'../../public/buy-comics-merchandise.png',
                        name:'DC MERCHANDISE',
                    },
                    {
                        img:'../../public/buy-comics-subscriptions.png',
                        name:'SUBSCRITION',
                    },
                    {
                        img:'../../public/buy-comics-shop-locator.png',
                        name:'COMIC SHOP LOCATOR',
                    },
                    {
                        img:'../../public/buy-dc-power-visa.svg',
                        name:'DC POWER VISA',
                    }


                ]
                    
                
            }
        }

    }

</script>

<template>

<div class="merch">
    <div class="list">
        <ul>
            <li v-for="currentLink in links">
                <div class="box-img">
                    <img :src="currentLink.img" alt="#">
                </div>
                <strong>{{currentLink.name}}</strong>
            </li>
        </ul>
    </div>
</div>

</template>

<style>

.merch{

display: flex;
justify-content: center;
align-items: center;

width: 100%;

background-color: #0c7cec;

padding: 50px 0;

.list{

    width: 80%;

    ul{

        display: flex;
        justify-content: space-between;
        align-items: center;

        list-style-type: none;

        li{

            display: flex;
            align-items: center;

            gap: 15px;

            padding: 0 25px;

            .box-img{
                height: 65px;

                img{
                    height: 100%;
                }

            }


        }
    }

}

}

</style>
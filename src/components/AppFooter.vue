<script>

    export default {
        
        name: 'AppFooter',

        data() {
            return {
                
                dcComics: [
                    {
                        linkComics: 'Characters',
                    },
                    {
                        linkComics: 'Comics',
                    },
                    {
                        linkComics: 'Movies',
                    },
                    {
                        linkComics: 'TV',
                    },
                    {
                        linkComics: 'Games',
                    },
                    {
                        linkComics: 'Videos',
                    },
                    {
                        linkComics: 'News',
                    },
                ],
        
                shop: [
                    {
                        linkShop: 'Shop DC',
                    },
                    {
                        linkShop: 'Shop DC Collectibles',
                    },
                ],
        
                dc: [
                    {
                        linkDc: 'Terms Of Use',
                    },
                    {
                        linkDc: 'Privacy Policy (New)',
                    },
                    {
                        linkDc: 'Ad Choise',
                    },
                    {
                        linkDc: 'Advertising',
                    },
                    {
                        linkDc: 'Jobs',
                    },
                    {
                        linkDc: 'Subscriptions',
                    },
                    {
                        linkDc: 'Talent Workshops',
                    },
                    {
                        linkDc: 'CPSC Certificates',
                    },
                    {
                        linkDc: 'Ratings',
                    },
                    {
                        linkDc: 'Shop Help',
                    },
                    {
                        linkDc: 'Contact Us',
                    },
                ],
        
                sites: [
                    {
                        linkSites: 'DC',
                    },
                    {
                        linkSites: 'MAD Magazine',
                    },
                    {
                        linkSites: 'DC Kids',
                    },
                    {
                        linkSites: 'DC Universe',
                    },
                    {
                        linkSites: 'DC Power Visa',
                    },
                ],

                social: [
                    {
                        imgSocial: '../../public/footer-facebook.png'
                    },
                    {
                        imgSocial: '../../public/footer-twitter.png'
                    },
                    {
                        imgSocial: '../../public/footer-youtube.png'
                    },
                    {
                        imgSocial: '../../public/footer-pinterest.png'
                    },
                    {
                        imgSocial: '../../public/footer-periscope.png'
                    },
                ],

            }
        }

        
    }

</script>

<template>
<div class="footer">
    <div class="jumbo">
        <div class="box-img">
            <img src="../../public/dc-logo-bg.png" alt="#">
        </div>
        <div class="list">
            <div>
                <div>
                    <ul>
                        <strong>DC COMICS</strong>
                        <li v-for="currentComics in dcComics">
                            {{currentComics.linkComics}}
                        </li>
                    </ul>
                </div>
                <div>
                    <ul>
                        <strong>SHOP</strong>
                        <li v-for="currentShop in shop">{{ currentShop.linkShop }}</li>
                    </ul>
                </div>
            </div>
            <div>
                <ul>
                    <strong>DC</strong>
                    <li v-for="currentDc in dc">{{ currentDc.linkDc }}</li>
                </ul>
            </div>
            <div>
                <ul>
                    <strong>SITES</strong>
                    <li v-for="currentSites in sites">{{ currentSites.linkSites }}</li>
                </ul>
            </div>
        </div>
    </div>
    <div class="social">
        <div class="btn">
            <strong>SIGN-UP NOW</strong>
        </div>
        <div class="followUs">
            <ul>
                <li><strong>FOLLOW US</strong></li>
                <li v-for="currentSocial in social">
                    <img :src="currentSocial.imgSocial" alt="#">
                </li>
            </ul>
        </div>
    </div>
</div>

</template>

<style lang="scss">

@use '../../src/style/variables' as *;

.footer{


    background-color: #242424;

    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    
    .jumbo{

        position: relative;

        overflow: hidden;

        width: 100%;

        background-image: url(../../public/footer-bg.jpg);

        background-size: cover;

        display: flex;
        justify-content: center;

        .box-img{

            position: absolute;

            top: 50%;
            transform: translateY(-50%);
            right: 15%;

        }

        .list{

            width: 80%;

            display: flex;
            gap: 40px;

            padding: 45px 0;

            ul{
                list-style-type: none;

                margin-bottom: 25px;

                
                strong{
                    font-size: 25px;
                    display: block;

                    margin-bottom: 15px;
                }

                li{
                    cursor: pointer;

                    user-select: none;


                    color: #999;
                }
            }

        }
    
    
    }

    .social{
        
        width: 80%;

        display: flex;
        justify-content: space-between;
        align-items: center;

        padding: 24px 0;


        .btn{

            display: flex;
            justify-content: center;
            align-items: center;

            user-select: none;
            cursor: pointer;

            border: 5px solid $primarycolor;
            
            padding: 20px 25px;
        }

        .followUs{

            display: flex;


            ul{
                display: flex;
                align-items: center;

                gap: 20px;

                list-style-type: none;

                li{
                    
                    user-select: none;

                    display: flex;
                    justify-content: center;
                    align-items: center;

                    img{
                        cursor: pointer;
                    }

                    strong{
    
                        color: $primarycolor;
                        font-size: 25px;
    
                    }

                }
                
            }
        }



    }

}


</style>
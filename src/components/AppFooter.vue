<script>
    import AppMerchandise from './AppMerchandise.vue';

    export default {
        components: {
            AppMerchandise,

        },

        link: 'AppFooter',

        data() {

            return {
                
                linkList: [
                    {
                        title: 'DC COMICS',
                        links:['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News']
                    },
                    {
                        title: 'SHOP',
                        links:['Shop DC', 'Shop DC Collectibles']
                    },
                    {
                        title: 'DC',
                        links:['Terms of Use', 'Privacy Policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshop', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us']
                    },
                    {
                        title: 'SITES',
                        links:['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
                    },
            ],
            

                icons: ['/img/footer-facebook.png', '/img/footer-twitter.png', '/img/footer-youtube.png', '/img/footer-pinterest.png', '/img/footer-periscope.png']
            }
        }
    }
</script>

<template>
    <AppMerchandise></AppMerchandise>
    <footer>
        <div class="container">
            <div class="footer-links">
                <div v-for="currentList in linkList" class="link-list">
                    <h3>{{ currentList.title }}</h3>
                    <ul>
                        <li v-for="currentLink in currentList.links">{{ currentLink }}</li>                       
                    </ul>
                </div>
            </div>
            <img src="/img/dc-logo-bg.png" alt="">
        </div>
    </footer>
    <div class="social">
        <div class="container">
            <div class="sign-up">
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="follow">
                <h3>FOLLOW US</h3>
                <img v-for="icon in icons" :src=" icon " alt="">
            </div>
        </div>
    </div>
</template>

<style lang="scss">
@use '../styles/main' as *;

    footer{
        position: relative;
        width: 100%;
        height: 380px;
        background-image: url(./img/footer-bg.jpg);
        background-size: cover;
        overflow: hidden;

        .container{
            display: $primaryFlex;
            justify-content: space-between;
            width: $primaryDimension;
            margin-left: auto;
            margin-right: auto;
            height: 100%;
            padding: 0px;

            .footer-links{
                display: $primaryFlex;
                flex-direction: column;
                flex-wrap: wrap;
                gap: 30px;

                height: 100%;
                padding: 25px 0;

                .link-list{
                    display: $primaryFlex;
                    flex-direction: column;
                    gap: 10px;

                    ul{
                        display: $primaryFlex;
                        flex-direction: column;
                        align-items: flex-start;
                        gap: 5px;
                        list-style-type: none;
                        font-size: 12px;
                    }

                    .shop{

                        h3{
                            padding: 10px 0;
                        }
                    }
                }

            }

            img{
                position: absolute;
                top: -20%;
                right: 200px;
            }

        }

    }
    .social{
        width: 100%;
        background-color: #303030;

        .container{
            display: $primaryFlex;
            justify-content: space-between;
            align-items: center;
            width: $primaryDimension;
            margin-left: auto;
            margin-right: auto;
            padding: 20px 0;

            .sign-up{
                button{
                    background-color: transparent;
                    color: white;
                    padding: 15px 10px;
                    border: 1px solid $primaryColor;
                }
            }

            .follow{
                display: $primaryFlex;
                align-items: center;
                gap: 15px;

                h3{
                    color: $primaryColor;
                }
            }
        }
    }
</style>
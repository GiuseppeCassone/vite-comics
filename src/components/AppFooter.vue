<script>
    import AppMerchandise from './AppMerchandise.vue';

    export default {
        components: {
            AppMerchandise,

        },

        link: 'AppFooter',

        data() {

            return {
                
                lists: [
                    {
                        title: 'DC COMICS',
                        link: ['Character', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News']
                    },
                    {
                        title: 'DC',
                        link: ['Therms Of Use', 'Privacy policy (New)', 'Ad Chokes', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us']
                    },
                    {
                        title: 'SITES',
                        link: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
                    },
    
                ],

                icons: ['/img/footer-facebook.png', '/img/footer-twitter.png',]
            }
        }
    }
</script>

<template>
    <AppMerchandise></AppMerchandise>
    <footer>
        <div class="container">
            <div class="footer-links">
                <div class="link-list" v-for="currentList in lists">
                    <h3>{{ currentList.title }}</h3>
                    <ul>
                        <li v-for="currentLink in currentList.link">{{ currentLink }}</li>                       
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
                <img src="/img/footer-facebook.png" alt="">
            </div>
        </div>
    </div>
</template>

<style lang="scss">

    footer{
        position: relative;
        width: 100%;
        height: 370px;
        background-image: url(./img/footer-bg.jpg);
        background-size: cover;
        overflow: hidden;

        .container{
            display: flex;
            justify-content: space-between;
            width: 70%;
            margin-left: auto;
            margin-right: auto;
            padding: 0px;

            .footer-links{
                display: flex;
                gap: 30px;
                padding: 45px 0;

                .link-list{
                    display: flex;
                    flex-direction: column;
                    gap: 10px;

                    ul{
                        display: flex;
                        flex-direction: column;
                        align-items: flex-start;
                        gap: 5px;
                        list-style-type: none;
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
            display: flex;
            justify-content: space-between;
            align-items: center;
            width: 70%;
            margin-left: auto;
            margin-right: auto;
            padding: 20px 0;

            .sign-up{
                button{
                    background-color: transparent;
                    color: white;
                    padding: 15px 10px;
                    border: 1px solid #0282F9;
                }
            }

            .follow{
                display: flex;
                align-items: center;
                gap: 15px;

                h3{
                    color: #0282F9;
                }
            }
        }
    }
</style>
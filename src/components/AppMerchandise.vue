<script>
    export default {
        icons: 'AppMerchandise',

        data() {

            return {
                item: [ 
                    {
                        image: './img/buy-comics-digital-comics.png',
                        link: 'DIGITAL COMICS',
                    },
                    {
                        image: './img/buy-comics-merchandise.png',
                        link: 'DC MERCHANDISE',
                    },
                    {
                        image: './img/buy-comics-subscriptions.png',
                        link: 'SUBSCRIPTION',
                    },
                    {
                        image: './img/buy-comics-shop-locator.png',
                        link: 'COMIC SHOP LOCATOR',
                    },
                    {
                        image: './img/buy-dc-power-visa.svg',
                        link: 'DC POWER VISA',
                    },
                ]

            }
        }
    }
</script>

<template>
    <section class="merchandise">
        <div class="container">
            <div class="icon-links" v-for="currentItem in item">
                <img :src="currentItem.image" alt="">
                <span>{{ currentItem.link }}</span>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
@use '../styles/main' as *;

    .merchandise{
        width: 100%;
        background-color: $primaryColor;

        .container{
            display: flex;
            justify-content: space-between;
            width: $primaryDimension;
            margin-left: auto;
            margin-right: auto;
            gap: 20px;
            padding: 30px;

            .icon-links{
                display: flex;
                align-items: center;
                gap: 10px;

                img{
                    width: auto;
                    height: 55px;
                }
            }

            .icon-links:last-child img{
                width: 50px;
                height: auto;
            }

        }
    }
</style>
<script>
    export default {
        icons: 'AppMerchandise',
    }
</script>

<template>
    <section class="merchandise">
        <div class="container">
            <div class="icon-links">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>DIGITAL COMICS</span>
            </div>
            <div class="icon-links">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>DC MERCHANDISE</span>
            </div>
            <div class="icon-links">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>SUBSCRIPTION</span>
            </div>
            <div class="icon-links">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>COMIC SHOP LOCATOR</span>
            </div>
            <div class="icon-links">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>DC POWER VISA</span>
            </div>
        </div>
    </section>
</template>

<style lang="scss">

    .merchandise{
        width: 100%;
        background-color: #0282F9;

        .container{
            display: flex;
            justify-content: space-between;
            width: 70%;
            margin-left: auto;
            margin-right: auto;
            gap: 20px;
            padding: 30px;

            .icon-links{
                display: flex;
                align-items: center;
                gap: 10px;

                img{
                    width: 45px;
                    height: 55px;
                }
            }

        }
    }
</style>
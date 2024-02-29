<script>

    export default {
        link: 'AppFooter',
    }
</script>

<template>
    <footer>
        <div class="container">
            <div class="footer-links">
                <div class="link-list">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                    </ul>
                </div>
                <div class="link-list">
                    <h3>DC</h3>
                    <ul>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                    </ul>
                </div>
                <div class="link-list">
                    <h3>SITE</h3>
                    <ul>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                        <li>uno</li>
                    </ul>
                </div>
            </div>
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
    </footer>
    <div class="social">
        <div class="container">
            <div class="sign-up">
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="follow">
                <h3>FOLLOW US</h3>
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-facebook.png" alt="">
            </div>
        </div>
    </div>
</template>

<style lang="scss">

    footer{
        position: relative;
        width: 100%;
        height: 370px;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        overflow: hidden;

        .container{
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
            align-items: center;

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
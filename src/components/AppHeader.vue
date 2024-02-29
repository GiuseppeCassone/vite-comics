<script>

    export default {
        name: 'AppHeader',

        data() {
            return {
                navlinks: [
                    'CHARACTERS',
                    'COMICS',
                    'MOVIES',
                    'TV',
                    'GAMES',
                    'COLLECTIBLES',
                    'VIDEOS',
                    'FANS',
                    'NEWS',
                    'SHOP'
                ],

                activeLinkIndex: 1,
            }
        }
    }


</script>

<template>
    <header>
        <nav class="container">
            <img src="/img/dc-logo.png" alt="">
            <ul>
                <li v-for="(currentNavLinks, index) in navlinks" :class="index == activeLinkIndex ? 'active' : ''">{{ currentNavLinks }}</li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss">
@use '../styles/main' as *;

    header{
        width: 100%;
        background-color: white;
        color: black;

        .container{
            display: flex;
            justify-content: space-between;
            width: $primaryDimension;
            margin-left: auto;
            margin-right: auto;
            // padding: 20px 0;

            img{
                padding: 20px 0;
            }
        
            ul{
                display: flex;
                align-items: center;
                gap: 25px;
                list-style-type: none;
                
                li{
                    font-size: 12px;
                    font-weight: bold;
                    padding: 62px 0;

                    &.active{
                        color: $primaryColor;
                        border-bottom: 4px solid $primaryColor;
                    }
                }

            }
        }
        
        
    }

</style>

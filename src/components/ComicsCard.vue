<script>

    export default {
        name: 'ComicsCard',

        props: {
            comicTitle: String,
            comicImg: String
        },
        
    }
</script>

<template>
     <div class="card">
        <img crossorigin="anonymous" :src="comicImg" :alt="comicTitle">
        <h4>{{ comicTitle }}</h4>
    </div>
</template>

<style lang="scss">

        .card{
            width: calc(100% / 6 - 25px / 6 * 5);
            margin-bottom: 15px;

                img{
                    width: 180px;
                    height: 180px;
                    margin-bottom: 10px;
                    object-fit: cover;
                    object-position: top;
                }

                h4{
                    text-transform: uppercase;
                    font-size: 12px;
                }
        }

</style>
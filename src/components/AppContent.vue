<script>
    export default {
        title: 'AppContent',
    }
</script>

<template>
    <section class="content">
        <img src="../../public/img/jumbotron.jpg" alt="jumbotron">
        <div class="container">
            <h1> Content goes here </h1>
        </div>
    </section>
</template>

<style lang="scss">
@use '../styles/main' as *;

    .content{
        width: 100%;

        img{
            width: 100%;
            height: 400px;
            object-fit: cover;
            object-position: top;
        }
        
        .container{
            display: $primaryFlex;
            justify-content: space-between;
            width: $primaryDimension;
            margin-left: auto;
            margin-right: auto;
            padding: 20px 0;

            h1{
                font-size: 40px;
            }
        }
    }

</style>
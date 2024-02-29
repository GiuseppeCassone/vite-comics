<script>
    export default {
        title: 'AppContent',
    }
</script>

<template>
    <section class="content">
        <div class="container">
            <h1> Content goes here </h1>
        </div>
    </section>
</template>

<style lang="scss">
@use '../styles/main' as *;

    .content{
        width: 100%;
        padding: 40px 0;
        
        .container{
            display: flex;
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
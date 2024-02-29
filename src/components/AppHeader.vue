<script>

    export default {
        name: 'AppHeader',
    }

</script>

<template>
    <header>
        <nav class="container">
            <img src="../assets/img/dc-logo.png" alt="">
            <ul>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss">
    header{
        width: 100%;
        padding: 20px 0;
        background-color: white;
        color: black;

        .container{
            display: flex;
            justify-content: space-between;
            width: 70%;
            margin-left: auto;
            margin-right: auto;

            ul{
                display: flex;
                align-items: center;
                gap: 15px;
                list-style-type: none;
            }
        }


    }
</style>

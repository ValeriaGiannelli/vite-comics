<script>
    export default{
        name: "Header",
    }

</script>

<template>
    <div class="container_menu">
        <!-- logo -->
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
        </div>

        <!-- menu navigazione -->
        <nav>
            <ul>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
            </ul>
        </nav>
    </div>

    

</template>

<style lang="scss" scoped>
.container_menu{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    margin: 0 auto;
    padding: 20px;

    .logo{
        max-width: 80px;
    }

    ul{
        display: flex;
        gap: 10px;
        font-size: 12px;
        list-style-type: none;
    }
}


</style>
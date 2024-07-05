<script>
    export default{
        name: "Header",
    }

</script>

<template>
    <div class="container">
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
.container{
    justify-content: space-between;
    padding: 20px 0;

    .logo{
        max-width: 80px;
    }

    ul{
        display: flex;
        gap: 10px;
        font-size: 12px;

        a{
            color: black;
        }
    }
}


</style>
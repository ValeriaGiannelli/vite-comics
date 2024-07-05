<script>
    export default{
        name: "Footer",
    }

</script>


<template>
        <div class="up">

            <div class="container">

                <div class="single-element">
                    <!-- icona del link -->
                    <div class="img">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    </div>

                    <!-- link -->
                    <a href="#">DIGITAL COMICS</a>
                </div>

                <div class="single-element">
                    <!-- icona del link -->
                    <div class="img">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    </div>

                    <!-- link -->
                    <a href="#">DIGITAL COMICS</a>
                </div>

                <div class="single-element">
                    <!-- icona del link -->
                    <div class="img">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    </div>

                    <!-- link -->
                    <a href="#">DIGITAL COMICS</a>
                </div>

                <div class="single-element">
                    <!-- icona del link -->
                    <div class="img">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    </div>

                    <!-- link -->
                    <a href="#">DIGITAL COMICS</a>
                </div>

                <div class="single-element">
                    <!-- icona del link -->
                    <div class="img">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    </div>

                    <!-- link -->
                    <a href="#">DIGITAL COMICS</a>
                </div>
                

            </div>

        </div>

        <div class="link-utili">

            <div class="container">

            </div>

        </div>

        <div class="down">

            <div class="container">

            </div>

        </div>



</template>

<style lang="scss" scoped>
 @use '../styles/partials/mixins' as *;

    .up{
        background-color: blue;
        display: flex;
        align-items: center;

        // debug
        height: 150px;
    }

    .container{
        justify-content: space-around
    }

    .single-element{
       @include flex-center;
    }

    .img{
        width: 50px;
    }

    a{
        color: white;
        padding-left: 10px;
    }
</style>
<script>
    export default{
        name: "Footer",
    }

</script>


<template>

        <!-- parte alta del merchandise -->
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

        <!-- link utili -->
        <div class="link-utili">

            <div class="container">

                <!-- parte dei link -->
                <div class="links">

                    <!-- colonna -->
                    <div class="col-link">
                        <ul>
                            <!-- titolo -->
                            <li class="title">
                                DC COMICS
                            </li>
                            
                            <!-- link -->
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>

                            <!-- titolo -->
                            <li class="title">
                                DC COMICS
                            </li>

                            <!-- link -->
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                        </ul>
                    </div>

                    <!-- colonna -->
                    <div class="col-link">
                        <ul>
                            <!-- titolo -->
                            <li class="title">
                                DC COMICS
                            </li>
                            
                            <!-- link -->
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                        </ul>
                    </div>

                    <!-- colonna -->
                    <div class="col-link">
                        <ul>
                            <!-- titolo -->
                            <li class="title">
                                DC COMICS
                            </li>
                            
                            <!-- link -->
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                        </ul>
                    </div>


                </div>

                <!-- parte del logo -->
                 <div class="log-bg">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                 </div>

            </div>

        </div>


        <!-- sing-up e follow us -->
        <div class="down">

            <div class="container">

            </div>

        </div>



</template>

<style lang="scss" scoped>
 @use '../styles/partials/mixins' as *;

//  parte alta
    .up{
        background-color: blue;
        display: flex;
        align-items: center;
        min-height: 150px;
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

// link utili
    .link-utili{
        background-image: url("../assets/img/footer-bg.jpg");

        .container{
            justify-content: space-between;
        }

        li{
            padding: 3px 0;
        }

        a{
            padding: 0;
            color: gray;
        }

        // titolo della colonna dei link
        .title{
            color: white;
            padding: 10px 0;
        }
    }
    

    .links{
        display: flex;
    }

    .col-link{
        min-width: 140px;
    }

// logo
    .log-bg{
        height: 400px;
        img{
            height: 100%;
        }
    }

// sing-up e follow us
</style>
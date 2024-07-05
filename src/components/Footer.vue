<script>
    export default{
        name: "Footer",
        
        data(){
            return{
                // PAGINE DI SHOP ECC
                pages: [
                    {
                        title: "DIGITAL COMICS",
                        path: "buy-comics-digital-comics.png",
                    },
                    {
                        title: "DC MERCHANDISE",
                        path: "buy-comics-merchandise.png",
                    },
                    {
                        title: "SUBSCRIPTION",
                        path: "buy-comics-subscriptions.png",
                    },
                    {
                        title: "COMIC SHOP LOCATOR",
                        path: "buy-comics-shop-locator.png",
                    },
                    {
                        title: "DC POWER VISA",
                        path: "buy-dc-power-visa.svg",
                    },
                ],
                
                // link utili
                dcComics: [
                    {
                        title: "Characters",
                        url: "#",
                    },
                    {
                        title: "Comics",
                        url: "#",
                    },
                    {
                        title: "Movies",
                        url: "#",
                    },
                    {
                        title: "TV",
                        url: "#",
                    },
                    {
                        title: "Games",
                        url: "#",
                    },
                    {
                        title: "Videos",
                        url: "#",
                    },
                    {
                        title: "News",
                        url: "#",
                    },
                ],

                shop: [
                    {
                        title: "Shop DC",
                        url: "#",
                    },
                    {
                        title: "Shop DC Collectibles",
                        url: "#",
                    },
                ],

                dc: [
                    {
                        title: "Terms Of Use",
                        url: "#",
                    },
                    {
                        title: "Privace policy(New)",
                        url: "#",
                    },
                    {
                        title: "Ad Choices",
                        url: "#",
                    },
                    {
                        title: "Advertising",
                        url: "#",
                    },
                    {
                        title: "Jobs",
                        url: "#",
                    },
                    {
                        title: "Supscriptions",
                        url: "#",
                    },
                    {
                        title: "Talent Workshop",
                        url: "#",
                    },
                    {
                        title: "CPSC Certificates",
                        url: "#",
                    },
                    {
                        title: "Ratings",
                        url: "#",
                    },
                    {
                        title: "Shop Help",
                        url: "#",
                    },
                    {
                        title: "Contact Us",
                        url: "#",
                    },
                ],

                sites: [
                    {
                        title: "DC",
                        url: "#",
                    },
                    {
                        title: "MAD Magazine",
                        url: "#",
                    },
                    {
                        title: "DC Kids",
                        url: "#",
                    },
                    {
                        title: "DC Universe",
                        url: "#",
                    },
                    {
                        title: "DC Power Visa",
                        url: "#",
                    },
                ],
            }
        },
        methods:{
            getImagePath: function(imgPath){
                return new URL(imgPath, import.meta.url).href;
            }
        }
    }

</script>


<template>

        <!-- parte alta del merchandise -->
        <div class="up">

            <div class="container">

                <div class="single-element" v-for="(page, index) in pages" :key="index">
                    <!-- icona del link -->
                    <div class="imgagine">
                        <img :src="getImagePath(`../assets/img/${page.path}`)" :alt="page.title">
                    </div>

                    <!-- link -->
                    <a href="#">{{page.title}}</a>
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
                            <li v-for="(link, index) in dcComics" :ket="index">
                                <a :href="link.url">{{link.title}}</a>
                            </li>


                            <!-- titolo -->
                            <li class="title">
                               SHOP
                            </li>

                            <!-- link -->
                            <li v-for="(link, index) in shop" :ket="index">
                                <a :href="link.url">{{link.title}}</a>
                            </li>

                        </ul>
                    </div>

                    <!-- colonna -->
                    <div class="col-link">
                        <ul>
                            <!-- titolo -->
                            <li class="title">
                                DC
                            </li>
                            
                            <!-- link -->
                            <li v-for="(link, index) in dc" :ket="index">
                                <a :href="link.url">{{link.title}}</a>
                            </li>

                        </ul>
                    </div>

                    <!-- colonna -->
                    <div class="col-link">
                        <ul>
                            <!-- titolo -->
                            <li class="title">
                                SITES
                            </li>
                            
                            <!-- link -->
                            <li v-for="(link, index) in sites" :ket="index">
                                <a :href="link.url">{{link.title}}</a>
                            </li>
                            
                        </ul>
                    </div>


                </div>

                <!-- parte del logo -->
                 <div class="log-bg">
                    <!-- <img src="../assets/img/dc-logo-bg.png" alt=""> -->
                 </div>

            </div>

        </div>


        <!-- sing-up e follow us -->
        <div class="down">

            <div class="container">

                <button>SING-UP NOW!</button>

                <div class="follow">
                    <span>FOLLOW US</span>
                    <a href="#">
                        <img src="../assets/img/footer-facebook.png" alt="icona facebook">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-twitter.png" alt="icona facebook">
                        
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-youtube.png" alt="icona facebook">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-pinterest.png" alt="icona facebook">
                    </a>
                    <a href="#">
                        
                        <img src="../assets/img/footer-periscope.png" alt="icona facebook">
                    </a>
                </div>

            </div>

        </div>



</template>

<style lang="scss" scoped>
 @use '../styles/partials/mixins' as *;

//  parte alta
    .up{
        background-color: #0f82f7;
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

    .imgagine{
        width: 50px;
        height: 50px;

        img{
            height: 100%;
            object-fit: contain;
        }
    }

    a{
        color: white;
        padding-left: 10px;
    }

// link utili
    .link-utili{
        background-image: url("../assets/img/dc-logo-bg.png"), url("../assets/img/footer-bg.jpg");
        background-size: 10% cover;
        background-position-x: 80%;
        background-position-y: center;
        background-repeat: no-repeat;

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
        padding-right:30px;
    }

// logo
    .log-bg{
        height: 400px;
        img{
            height: 100%;
        }
    }

// sing-up e follow us
    .down{
        background-color: #2f2f2f;
        min-height: 150px;
        @include flex-center;
        
        .container{
            justify-content: space-between;

            button{
                color: white;
                font-size: 20px;
                padding: 15px;
                border: 2px solid #0f82f7;
                background-color: #2f2f2f;
            }
        }
    }

    .follow{
        @include flex-center;

        span{
            color: #0f82f7;
        }

        i{
            color: #787878;
        }
    }
</style>
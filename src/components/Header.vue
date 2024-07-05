<script>
    export default{
        name: "Header",

        data(){
            return{
                navLinks: [
                    {
                        title: "CHARACTERS",
                        url: "#",
                        selected: false
                    },
                    {
                        title: "COMICS",
                        url: "#",
                        selected: true
                    },
                    {
                        title: "MOVIES",
                        url: "#",
                        selected: false
                    },
                    {
                        title: "TV",
                        url: "#",
                        selected: false
                    },
                    {
                        title: "GAMES",
                        url: "#",
                        selected: false
                    },
                    {
                        title: "COLLECTIBLES",
                        url: "#",
                        selected: false
                    },
                    {
                        title: "VIDEOS",
                        url: "#",
                        selected: false
                    },
                    {
                        title: "FANS",
                        url: "#",
                        selected: false
                    },
                    {
                        title: "NEWS",
                        url: "#",
                        selected: false
                    },
                    {
                        title: "SHOP",
                        url: "#",
                        selected: false
                    },
                ]
            }
        }
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
                <li v-for="(link, index) in navLinks" :key="index">
                    <a :href="link.url" :class="{active: link.selected}">{{ link.title }}</a>
                </li>
            </ul>
        </nav>
    </div>

    

</template>

<style lang="scss" scoped>
.container{
    justify-content: space-between;
    min-height: 120px;

    .logo{
        max-width: 80px;
    }

    ul{
        display: flex;
        gap: 10px;
        font-size: 12px;

        li{
            height: 120px;
            display: flex;
            align-items: center;
        }

        a{
            color: black;
            min-height: 120px;
            display: flex;
            align-items: center;

            &.active{
            color: #0f82f7;
            border-bottom: 5px solid #0f82f7;
}
        }
    }
}




</style>
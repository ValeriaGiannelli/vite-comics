<script>
export default{
    name: "ListComics",
    props:{
        singleComic: Object,
    }
}

</script>


<template>
    <!-- card con immagine fumetto e titolo -->
    <div class="card">
        <!-- immagine che andrà gestita con props -->
        <div>
            <img :src="singleComic.thumb" :alt="singleComic.series">
        </div>
        <!-- titolo del fumetto gestito con props -->
        <h5>{{singleComic.series}}</h5>
    </div>

</template>

<style lang="scss" scoped>
// dimensioni totali card
.card{
    width: 200px;
    height: 250px;

    // dimensioni per il contenitore dell'immagine
    div{
        height: 200px;

        // caratteristiche dell'immagine
        img{
        height: 100%;
        object-fit: cover;
        object-position: top;
    }
    }

    h5{
        margin-top: 20px;
        text-transform: uppercase;
    }
    
}

</style>
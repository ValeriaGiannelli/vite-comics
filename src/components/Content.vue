<script>
import ListComics from './ListComics.vue';

 export default{
    name: "Content",
    components:{
        ListComics,
    }
 }

</script>


<template>
    <section class="contenuti">
        <div class="container">
            <ListComics/>
        </div>
    </section>

    <div class="contenuti more">
        <button>LOAD MORE</button>
    </div>

   
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
    .contenuti{
        background-color: #1c1c1c;
        display: flex;
        align-items: center;
        padding-top: 60px;

        // aggiunto un wrap alla condizione iniziale
        .container{
            flex-wrap: wrap;
            gap:50px 30px;
        }
    }

    .more{
        justify-content: center;
        button{
            background: $primary;
            padding: 10px 50px;
            color: $primary-text-color;
            border-color: $primary;
            margin-bottom: 20px;
        }
    }
</style>
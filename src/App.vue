<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Content from './components/Content.vue';

export default{
  name: "App",
  components: {
    Header,
    Footer,
    Content,
  }
}
</script>

<template>
  <Header/>
  
  <main>
    <Content/>
  </main>

  <Footer/>
</template>

<style lang="scss">
  @use './styles/general.scss' as *;
  h1,
  h2,
  h3,
  h4,
  h5,
  h6{
    color: white;
  }


</style>

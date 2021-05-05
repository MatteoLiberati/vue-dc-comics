<template>
  <div id="app">
    <!-- HEADER -->
    <Header/>
    <!-- MAIN -->
    <main>
      <Content/>
      <Banner/>
    </main>

    <!-- FOOTER -->
    <Footer/>
    <Bottomfixed/>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Content from "@/components/Content.vue";
import Banner from "@/components/Banner.vue";
import Footer from "@/components/Footer.vue";
import Bottomfixed from "@/components/Bottomfixed.vue";

export default {
  name: 'App',
  components: {
    Header,
    Content,
    Banner,
    Footer,
    Bottomfixed,
  }
}
</script>

<style lang="scss">
// GENERAL
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app{
  background-color:black;
  padding: 30px 0;
  font-family: 'Roboto', sans-serif;
}

.container{
  max-width: 1270px;
  margin: 0 auto;
}
</style>

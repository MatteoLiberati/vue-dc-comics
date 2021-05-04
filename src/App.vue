<template>
  <div id="app">
    <!-- HEADER -->
    <Header/>
    <!-- MAIN -->
    <main></main>

    <!-- FOOTER -->
    <footer></footer>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";

export default {
  name: 'App',
  components: {
    Header,
  }
}
</script>

<style lang="scss">
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

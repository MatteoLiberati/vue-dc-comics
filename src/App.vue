<template>
  <div id="app">
    <!-- HEADER -->
    <Header />
    <!-- MAIN -->
    <main>
      <Content />
      <Banner />
    </main>

    <!-- FOOTER -->
    <Footer />
    <Bottomfixed />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Content from "@/components/Content.vue";
import Banner from "@/components/Banner.vue";
import Footer from "@/components/Footer.vue";
import Bottomfixed from "@/components/Bottomfixed.vue";

export default {
  name: "App",
  components: {
    Header,
    Content,
    Banner,
    Footer,
    Bottomfixed,
  },
};
</script>

<style lang="scss">
// GENERAL STYLE
@import "./styles/generalstyle.scss";
// UTILITIES
@import "./styles/utilities.scss";
</style>

<template>
  <section>
    <!-- HERO -->
    <Hero/>
     <!-- CONTAINER -->
    <div class="container">
      <div class="current-series">CURRENT SERIES</div>
          <!-- CONTENT SPACE -->
          <Cardtemplate 
          v-for="(element,index) in Comics" 
          :key="element.series+index" 
          :details="element"/>
    </div>
    <!-- LOAD MORE -->
    <div>
      <button>LOAD MORE</button>
    </div>
  </section>
</template>

<script>
import Hero from "@/components/Hero";
import Cardtemplate from "@/components/Cardtemplate";
import Comics from "@/data/comics.js";

export default {
    name : "Content",
    components:{
        Hero,
        Cardtemplate,
    },
    data(){
      return{
        Comics,
      }
    }
}
</script>

<style scoped lang="scss">
@import "@/styles/vars.scss";
@import "../styles/content.scss";

</style>
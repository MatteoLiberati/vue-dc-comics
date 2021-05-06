<template>
  <div class="div">
      <div class="fixed-top">
          <div class="container">
              <div>
              <button>SING-UP NOW!</button>
              </div>
              <div>
                  <span>FOLLOW US</span>
                  <a v-for="(element,index) in social" :key="element.name + index" :href="element.link">
                      <img :src="element.img" :alt="element.name">
                  </a>
              </div>
          </div>
      </div>
      <div class="fixed-bottom"></div>
  </div>
</template>

<script>
import social from "@/data/social.js";

export default {
    name: "Bottomfixed",
    data(){
        return{
            social,
        }
    }
}
</script>

<style scoped lang="scss">
@import "../styles/fixedstyle.scss";
</style>
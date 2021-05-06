<template>
  <section>
      <!-- CONTAINER -->
      <div class="container">
          <!-- CARDS -->
          <div v-for="(element,index) in store" :key="element.name + index">
              <a href="#">
                  <img :src="element.img" :alt="element.name">
                  <span>{{element.name}}</span>
              </a>
          </div>
      </div>
  </section>
</template>

<script>
import store from "@/data/store.js"
export default {
    name: "Banner",
    data(){
        return{
            store,
        }
    }
}
</script>

<style scoped lang="scss">
@import "../styles/bannerstyle.scss";
</style>
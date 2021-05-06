<template>
  <footer>
      <div class="container">
          <div class="link-footer">
              <!-- COL SX -->
              <section class="col-xs">
                  <!-- LIST TOP SX -->
                  <h3>dc comics</h3>
                  <ul>
                        <li v-for="(element,index) in dcComics" :key="element.name+index">
                             <a :href="element.link">{{element.name}}</a>
                        </li>
                  </ul>
                  <!-- LIST BOTTOM SX -->
                  <h3>shops</h3>
                  <ul>
                        <li v-for="(element,index) in shops" :key="element.name+index">
                            <a :href="element.link">{{element.name}}</a>
                        </li>
                  </ul>
              </section>
              <!-- COL CENTRE -->
              <section class="col-c">
                  <!-- LIST CENTRE -->
                  <h3>dc</h3>
                  <ul>
                        <li v-for="(element,index) in dc" :key="element.name+index">
                            <a :href="element.link">{{element.name}}</a>
                        </li>
                  </ul>
              </section>
              <!-- COL DX -->
              <section class="col-dx">
                  <!-- LIST DX -->
                  <h3>sites</h3>
                  <ul>
                        <li v-for="(element,index) in sites" :key="element.name+index">
                            <a :href="element.link">{{element.name}}</a>
                        </li>
                  </ul>
              </section>
          </div>
          <!-- DIV TOTAL DX LOGO -->
          <div class="logo-footer">
              <img src="@/assets/images/dc-logo-bg.png" alt="logo footer">
          </div>
      </div>
  </footer>
</template>

<script>
import dcComics from "@/data/dcComics.js";
import shops from "@/data/shops.js";
import dc from "@/data/dcMenu.js";
import sites from "@/data/sitesMenu.js";

export default {
    name: "Footer",
    data(){
        return{
            dcComics,
            shops,
            dc,
            sites,
        }
    }
}
</script>

<style scoped lang="scss">
@import "../styles/mixins.scss";
@import "../styles/footerstyle.scss"
</style>
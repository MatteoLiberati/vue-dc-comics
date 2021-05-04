<template>
  <footer>
      <div class="container">
          <div class="link-footer">
              <!-- COL SX -->
              <section class="col-xs">
                  <h3>dc comics</h3>
                  <ul>
                      <li v-for="(element,index) in dcComics" :key="element+index">
                          <a href="#">{{element}}</a>
                      </li>
                  </ul>
                  <h3>shops</h3>
                  <ul>
                      <li v-for="(element,index) in shop" :key="element+index">{{element}}</li>
                  </ul>
              </section>
              <!-- COL CENTRE -->
              <section class="col-c">
                  <h3>dc</h3>
                  <ul>
                      <li v-for="(element,index) in dc" :key="element+index">{{element}}</li>
                  </ul>
              </section>
              <!-- COL DX -->
              <section class="col-dx">
                  <h3>sites</h3>
                  <ul>
                      <li v-for="(element,index) in sites" :key="element+index">{{element}}</li>
                  </ul>
              </section>
          </div>
          <div class="logo-footer">
              <img src="@/assets/images/dc-logo-bg.png" alt="logo footer">
          </div>
      </div>
  </footer>
</template>

<script>
export default {
    name: "Footer",
    data(){
        return{
            dcComics: ["Characthers","Comics","Movies","TV","Games","Videos","News"],
            shop: ["Shop DC","Shop DC Collectibles"],
            dc: ["Terms Of Use","Privacy policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
            sites: ["DC","MAD Magazine", "DC Kids", "DC Universe", "DC Power VIsa"],
        }
    }
}
</script>

<style scoped>
footer{
    /* background-image: url("C:/Users/Teo e Robi/Documents/Boolean Careers/lezione58 - nodejs, vue CLI, prompt comandi/vue-dc-comics/src/assets/images/footer-bg.jpg"); */
    background-image: url("../assets/images/footer-bg.jpg");
    max-height: 40vh;
    overflow: hidden;
}

.link-footer{
    display: flex;
    justify-content: space-between;
    padding: 20px;
    width: 30%;
}

.link-footer ul{
    list-style: none;
}

.link-footer a{
    color: grey;
    text-decoration: none;
}

.link-footer h3{
    color: #fff;
    text-transform: uppercase;
    margin-bottom: 10px;
}

.logo-footer{
    transform:translateY(-60px)
}

.container{
    display: flex;
    justify-content:space-between;
}

</style>
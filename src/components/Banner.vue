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
export default {
    name: "Banner",
    data(){
        return{
            store: [
                {
                    name: "digital comics",
                    img: require("../assets/images/buy-comics-digital-comics.png"),
                },
                {
                    name: "cd merchandise",
                    img: require("../assets/images/buy-comics-merchandise.png"),
                },
                {
                    name: "subscription",
                    img: require("../assets/images/buy-comics-subscriptions.png"),
                },
                {
                    name: "comic shop locator",
                    img: require("../assets/images/buy-comics-shop-locator.png"),
                },
                {
                    name: "dc power visa",
                    img: require("../assets/images/buy-dc-power-visa.svg"),
                },
            ]
        }
    }
}
</script>

<style scoped>
/* SECTION */
section{
    background-color:#0c7cec;
}

/* CONTAINER */
section .container{
    display: flex;
    justify-content:space-between;
    align-items: center;
}

/* CARDS */
.container div a{
    display:flex;
    align-items: center;
    padding: 70px 15px;
    text-decoration: none;
    transition: transform .3s;
}

.container div a:hover{
    transform: scale(1.1);
}

.container div img{
    height: 60px;
    margin-right: 10px;
}

.container div:last-child img{
    height: auto;
    width: 60px;
}

.container div span{
    text-transform: uppercase;
    color: #fff;
}


</style>
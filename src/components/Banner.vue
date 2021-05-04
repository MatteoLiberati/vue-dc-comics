<template>
  <section>
      <div class="container">
          <div v-for="(element,index) in store" :key="element.name + index">
              <img :src="'@/assets/images/'+element.img" :alt="element.name">
              <span>{{element.name}}</span>
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
                    img: "buy-comics-digital-comics.png",
                },
                {
                    name: "cd merchandise",
                    img: "buy-comics-merchandise.png",
                },
                {
                    name: "subscription",
                    img: "buy-comics-subscriptions.png",
                },
                {
                    name: "comic shop locator",
                    img: "buy-comics-shop-locator.png",
                },
                {
                    name: "dc power visa",
                    img: "buy-dc-power-visa.png",
                },
            ]
        }
    }
}
</script>

<style scoped>
section{
    background-color:#0c7cec;
}
section .container{
    display: flex;
}

.container div{
    padding: 70px 0;
}
</style>
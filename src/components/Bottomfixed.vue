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
                      <img :src="'/images/'+element.img" :alt="element.name">
                  </a>
              </div>
          </div>
      </div>
      <div class="fixed-bottom"></div>
  </div>
</template>

<script>
export default {
    name: "Bottomfixed",
    data(){
        return{
            social: [
                {
                    name: "Facebook",
                    img: "footer-facebook.png",
                    link: "/facebook"
                },
                {
                    name: "Twitter",
                    img: "footer-twitter.png",
                    link: "/twitter"
                },
                {
                    name: "Youtube",
                    img: "footer-youtube.png",
                    link: "/youtube"
                },
                {
                    name: "Pinterest",
                    img: "footer-pinterest.png",
                    link: "/pinterest"
                },
                {
                    name: "Periscope",
                    img: "footer-periscope.png",
                    link: "/periscope"
                },
                
            ]
        }
    }
}
</script>

<style scoped>
.div {
    position: fixed;
    left: 0;
    bottom: 0;
    width: 100%;
}
/* FIXED TOP */
.fixed-top{
    background-color: #303030;
}

.fixed-top .container{
    display: flex;
    justify-content: space-between;
}

.fixed-top .container button{
    border: 2px solid #0c7cec;
    text-transform: uppercase;
    color: #fff;
    padding: 14px 10px;
    font-size: 1.06rem;
    background-color: transparent;
    cursor: pointer;
    transition: transform .3s;
}

.fixed-top .container button:hover{
    transform: scale(1.1);
}

.fixed-top .container > div{
    display:flex;
    align-items: center;
    
}

.fixed-top .container > div span{
    color: #0c7cec;
    font-size: 1.3rem;
    font-weight: bold;
}

.fixed-top .container > div img{
    margin-left: 20px;
    padding: 40px 0;
    transition: transform .5s
}

.fixed-top .container > div img:hover{
    transform: rotate(360deg);
}

.fixed-bottom{
    height: 60px;
    background-color: black;
}
</style>
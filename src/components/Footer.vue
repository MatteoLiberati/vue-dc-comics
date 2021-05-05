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
export default {
    name: "Footer",
    data(){
        return{
            dcComics: [
                {
                    name: "Characthers",
                    link: "/characthers",
                },
                {
                    name: "Comics",
                    link: "/comics",
                },
                {
                    name: "Movies",
                    link: "/movies",
                },
                {
                    name:"TV",
                    link:"/tv",
                },
                {
                    name: "Games",
                    link: "/games",
                },
                {
                    name: "Videos",
                    link: "/videos",
                },
                {   name:"News",
                    link:"/news",
                },
            ],
            shops: [
                { 
                    name:"Shop DC",
                    link:"/shopdc",
                },
                {
                    name:"Shop DC Collectibles",
                    link: "/shopdccollectibles",
                },
            ],
            dc: [
                {
                    name: "Terms Of Use",
                    link: "/termsofuse",
                },
                {
                    name: "Ad Choices",
                    link: "/adchoices",
                },
                {
                    name: "Advertising",
                    link: "/advertising",
                },
                {
                    name: "Jobs",
                    link: "/jobs",
                },
                {
                    name: "Subscriptions",
                    link: "/subscriptions",
                },
                {
                    name: "Talent Workshops",
                    link: "/talentworkshops",
                },
                {
                    name: "CPSC Certificates",
                    link: "/cpsccertificates",
                },   
                {   name:"Ratings",
                    link:"/ratings",
                },
                {
                    name:"Shop Help",
                    link: "/shophelp",
                },
                {
                    name: "Contact Us",
                    link: "contactus",
                },
            ],
            sites: [
                {
                    name: "DC",
                    link: "/dc",
                },
                {   name: "MAD Magazine",
                    link: "/madmagazine",
                },
                {   name: "DC Kids",
                    link: "/dckids",
                },
                {   name: "DC Universe",
                    link: "/dcuniverse",
                },
                {   name: "DC Power VIsa",
                    link: "/dcpowervisa",
                },
            ],
        }
    }
}
</script>

<style scoped>
/* FOOTER */
footer{
    background-image: url("../assets/images/footer-bg.jpg");
    max-height: 50vh;
    overflow: hidden;
}

.container{
    display: flex;
    justify-content:space-between;
}

.link-footer{
    display: flex;
    justify-content: space-between;
    padding: 20px;
    width: 35%;
}

.link-footer ul{
    list-style: none;
}

.link-footer a{
    font-size: .8rem;
    color: grey;
    text-decoration: none;
    transition: color .3s;
}

.link-footer a:hover{
    color:#fff;
}

.link-footer h3{
    color: #fff;
    text-transform: uppercase;
    margin-bottom: 10px;
}
/* LIST BOTTOM SX */
.col-xs h3:not(:first-child){
    margin-top: 20px;
}

/* DIV TOTAL DX LOGO */
.logo-footer{
    transform:translateY(-60px)
}
</style>
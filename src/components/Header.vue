<template>
    <header>
        <!-- CONTAINER -->
        <div class="container">
            <!-- LOGO -->
            <div class="logo">
                <img src="@/assets/images/dc-logo.png" alt="logo">
            </div>
            <!-- NAV BAR -->
            <nav>
                <ul>
                    <li v-for="(element,index) in menu" :key="index">
                        <a :href="element.path">{{ element.name}}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    data(){
        return{
            menu : [
                {
                    name: "character",
                    path: "character.dc",
                },
                {
                    name: "comics",
                    path: "comics.dc",
                },
                {
                    name: "movies",
                    path: "movies.dc",
                },
                {
                    name: "tv",
                    path: "tv.dc",
                },
                {
                    name: "games",
                    path: "games.dc",
                },
                {
                    name: "collectibles",
                    path: "collectibles.dc",
                },
                {
                    name: "videos",
                    path: "videos.dc",
                },
                {
                    name: "fans",
                    path: "fans.dc",
                },
                {
                    name: "news",
                    path: "news.dc",
                },
                {
                    name: "shop",
                    path: "shop.dc",
                },
            ]
        }
    }
}
</script>

<style scoped>
header{
    background-color: #fff;
}

header .container{
    display: flex;
    justify-content: space-between;
}

/* LOGO */
header .logo{
    display:flex;
    align-items: center;
}

header .logo img{
    width: 80px;
}

/* NAVBAR */
ul{ 
    display: flex;
    list-style: none;
}

ul li a{ 
    padding: 15px;
    text-decoration: none;
    color: #000;
    text-transform: uppercase;
    font-size: .8rem;
    font-weight: bold;
}

ul li{
    border-bottom: 5px solid transparent;
    padding: 50px 0;
    transition: border-bottom .3s;
}

ul li:hover{
    border-bottom: 5px solid #0c7cec;
}


</style>
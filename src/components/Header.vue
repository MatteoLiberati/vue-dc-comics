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
import menu from '@/data/menu.js';
export default {
    name: "Header",
    data(){
        return{
            menu,
        }
    }
}
</script>

<style scoped lang="scss">
@import "../styles/vars.scss";
@import "../styles/headerstyle.scss";
</style>
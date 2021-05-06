<template>
    <a href="#" class="card">
        <div>
            <img :src="details.thumb" alt="">
        </div>
        <span>{{details.series}}</span>
    </a>
</template>

<script>
export default {
    props:["details"]
}
</script>

<style scoped lang="scss">
@import "../styles/cardstyle.scss";
</style>
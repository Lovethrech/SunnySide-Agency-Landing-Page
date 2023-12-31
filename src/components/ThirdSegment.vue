<script setup>
import GraphicDesign from "./GraphicDesign.vue";
import Photography from "./Photography.vue"
</script>

<template>
    <div class="third-segment-main-container">
        <div class="graphic-image-container">
            <GraphicDesign class="graphic-design"></GraphicDesign>
        </div>
        <div class="photography-container">
            <Photography class="photography"></Photography>
        </div>
    </div>
</template>

<style scoped>
.third-segment-main-container{
    display:flex;
    flex-wrap: nowrap;
    width:100%;
    height:100%;
}

.graphic-image-container{
    background: url("../assets/images/desktop/image-graphic-design.jpg") center center/auto no-repeat;
    background-size: cover;
    width:100%;
    height:70vh;
    text-align:center;
}
.graphic-design{
    padding:0 10vw;
    margin:50vh 0 0 0;
}

.photography-container{
    background: url("../assets/images/desktop/image-photography.jpg") center center/auto no-repeat;
    background-size: cover;
    width:100%;
    height:70vh;
    text-align:center;
}
.photography{
    padding:0 10vw;
    margin:50vh 0 0 0;
}
@media screen and (max-width:850px) {
    .third-segment-main-container{
        display:flex;
        flex-direction: column-reverse;
        flex-wrap: nowrap;
        width:100%;
        height:100%;
    }
    .graphic-design{
        margin:40vh 0 0 0;
    }
    .photography{
        margin:40vh 0 0 0;
    }
}
</style>
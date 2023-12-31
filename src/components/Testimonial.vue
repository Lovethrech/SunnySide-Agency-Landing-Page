<script setup>
import Emily from "./Emily.vue";
import Thomas from "./Thomas.vue";
import Jennie from "./Jennie.vue";
</script>
<template>
    <div class="main-testimonial-container">
        <div class="main-testimonial-container-title"><p>clients testimonials</p></div>
        <div class="client-container">
            <Emily></Emily>
            <Thomas></Thomas>
            <Jennie></Jennie>
        </div>
    </div>
</template>
<style scoped>
.main-testimonial-container{
    padding:10vh 0 20vh;
}
.main-testimonial-container-title{
    text-transform: uppercase;
    text-align:center;
    margin:3vh 0 8vh;
    color:hsl(210, 4%, 67%);
    font-weight:900;
    font-family: 'Fraunces', serif;
    letter-spacing: 1vh;
}
.client-container{
    display:flex;
    place-items:center;
    justify-content: center;
    gap:10px;
    padding:0 20vw;
}

@media screen and (max-width:850px) {

    .client-container{
        display:flex;
        flex-direction: column;
        padding:0 8vw;
    }
}
</style>
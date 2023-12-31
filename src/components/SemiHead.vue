<template>
    <div class="semi-head-content-container">
        <h1 class="semi-head-content-text">WE ARE CREATIVES</h1>
        <div class="arrow-container">
            <img src="../assets/images/icon-arrow-down.svg" alt="">
        </div>
    </div>
</template>
<style scoped>
.semi-head-content-container{
    margin:auto 0;
}
.semi-head-content-text{
    color:hsl(0, 100%, 100%);
    font-weight:900;
    font-size:4em;
    font-family: 'Fraunces', serif;
    letter-spacing: 1vw;
}
.arrow-container{
    text-align:center;
}

@media screen and (max-width:850px) {
    .semi-head-content-container{
        text-align:center;
    }
}
@media screen and (max-width: 465px) and (min-width: 301px) {
    .semi-head-content-text{
        font-size:2em;
    }
}
@media screen and (max-width:300px) {
    .semi-head-content-text{
        font-size: 14vw;
    }
}
</style>
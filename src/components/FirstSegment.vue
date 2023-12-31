<template>
    <div class="first-segment-main-container">
        <div class="first-segment-text">
            <h2 class="segment-title">Transform your brand</h2>
            <p  class="segment-paragraph">We are a full-service creative agency specializing in helping brands grow fast.
                Engage your clients through compelling visuals that do most of the marketing for you.
                <br><br><a href="" class="learn-link">Learn more</a>
            </p>
        </div>
        <div class="first-segment-image-container">
        </div>
    </div>
</template>
<style scoped>
.learn-link{
    text-transform: uppercase;
    text-decoration-color: hsla(51, 100%, 49%, 0.495);
    text-decoration-thickness: 5px;
    color:hsl(212, 27%, 19%);;
    font-weight:900;
    font-family: 'Barlow', sans-serif;
}
.learn-link:hover{
    text-decoration-color: hsl(51, 100%, 49%);
    transform: scaleX(1.1);
    transition:all .5s;
}
.first-segment-main-container{
    display:flex;
    flex-wrap: nowrap;
    width:100%;
    height:100%;
}
.segment-title{
    margin:0 6vw 2vh 10vw;
    font-size:2em;
    color:hsl(212, 27%, 19%);
    font-family: 'Fraunces', serif;
}
.segment-paragraph{
    margin: 0 10vw 0 10vw;
    color:hsl(232, 10%, 55%);
    font-family: 'Barlow', sans-serif;
}

.first-segment-text{
    background-color: hsl(0, 0%, 100%);
    display:flex;
    flex-direction:column;
    justify-content:center;
    width:100%;
}

.first-segment-image-container{
    background: url("../assets/images/desktop/image-transform.jpg") center center/auto no-repeat;
    background-size: cover;
    width:100%;
    height:70vh;
}

@media screen and (max-width:850px) {
    .first-segment-main-container{
        display:flex;
        flex-direction: column-reverse;
    }
    .first-segment-text{
        height:100%;
        padding:20vh 0;
    }
}
</style>
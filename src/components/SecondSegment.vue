<template>
    <div class="second-segment-main-container">
        <div class="second-segment-text">
            <h2 class="segment-title">Stand out to the right audience</h2>
            <p class="segment-paragraph">Using a collaborative formula of designers, researchers, photographers, videographers, and
                copywriters, we'll build and extend your brand in digital places.
                <br><br><a href="" class="learn-link">Learn more</a>
            </p>
        </div>
        <div class="second-segment-image-container">
        </div>
    </div>
</template>

<style scoped>
.learn-link{
    text-transform: uppercase;
    text-decoration-color: hsla(7, 99%, 70%, 0.495);
    text-decoration-thickness: 5px;
    color:hsl(212, 27%, 19%);
    font-weight:900;
    font-family: 'Barlow', sans-serif;
}
.learn-link:hover{
    text-decoration-color: hsl(7, 99%, 70%);
    transform: scaleX(1.1);
    transition:all .5s;
}
.second-segment-main-container{
    display:flex;
    flex-direction: row-reverse;
    width:100vw;
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
.second-segment-text{
    background-color: hsl(0, 0%, 100%);
    display:flex;
    flex-direction:column;
    justify-content:center;
    width:100%;
}
.second-segment-image-container{
    background: url("../assets/images/desktop/image-stand-out.jpg") center center/auto no-repeat;
    background-size: cover;
    width:100%;
    height:70vh;
}

@media screen and (max-width:850px) {
    .second-segment-main-container{
        display:flex;
        flex-direction: column-reverse;
        flex-wrap: nowrap;
        width:100%;
        height:100%;
    }
    .second-segment-text{
        height:100%;
        padding:20vh 0;
    }
}
</style>
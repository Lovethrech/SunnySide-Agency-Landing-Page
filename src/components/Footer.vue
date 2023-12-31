<template>
    <div class="footer-main-container">
        <div class="footer-logo-container">
            <img src="../assets/images/logo-coloured.svg" alt="">
        </div>
        <div class="footer-nav-container" style="margin:0;padding:0;">
            <ul class="footer-nav-list" style="padding:0;">
                <li class="footer-nav">About</li>
                <li class="footer-nav">Services</li>
                <li class="footer-nav">Projects</li>
            </ul>
        </div>
        <div class="footer-social-nav-container">
            <div class="social-nav"><i class='bx bxl-facebook-square'></i></div>
            <div class="social-nav"><i class='bx bxl-instagram-alt' ></i></div>
            <div class="social-nav"><i class='bx bxl-twitter' ></i></div>
            <div class="social-nav"><i class='bx bxl-pinterest' ></i></div>
        </div>
        <p class="challenge">Challenge by Frontend Mentor. Coded by 
            <a href="https://github.com/Lovethrech" 
            style="text-decoration:none; color:hsl(7, 99%, 70%);">
            Lovethrech</a>
        </p>
    </div>
</template>
<style scoped>
.footer-main-container{
    background-color: hsl(168, 47%, 68%);
    padding:10vh 0 3vh;
    text-align:center;
}
.footer-nav-list{
    list-style: none;
    display:flex;
    justify-content: center;
    gap:4vw;
    margin:2vh 0 4vh;
    font-family: 'Barlow', sans-serif;
}
.footer-nav:hover{
    cursor:pointer;
    color:hsl(0, 100%, 100%);
    transform:scale(1.05);
    transition: all .5s;
}
.footer-social-nav-container{
    display:flex;
    justify-content: center;
    gap:4vw;
}
.social-nav{
    margin:auto 0;
    font-size:28px;
}
.social-nav:hover{
    cursor:pointer;
    color:hsl(0, 100%, 100%);
    transform: scale(1.6);
    transition: all .5s;
}
.challenge{
    font-size:10px;
    text-align: center;
    letter-spacing:2px;
}

@media screen and (max-width:850px) {
    .footer-nav-list{
        justify-content: space-evenly;
        gap:4vw;
        margin:2vh 0 4vh;
    }
}
</style>
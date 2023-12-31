<template>
    <div class="dropdown-main-container">
        <ul class="head-nav-list">
            <li class="nav">About</li><br>
            <li class="nav">Services</li><br>
            <li class="nav">Projects</li><br>
            <li class="nav-contact" >CONTACT</li>
        </ul>
    </div>
</template>

<style scoped>
.head-nav-list{
    background-color: hsl(0, 100%, 100%);
    padding:6vh 0;
    margin: 0;
}
.head-nav-list{
    list-style: none;
    color:hsl(212, 27%, 19%);
    display:flex;
    flex-direction:column;
    text-align:center;
    padding:30px 100px;
}
.nav{
    margin:0 auto;
    font-family: 'Barlow', sans-serif;
}
.nav:hover{
    cursor:pointer;
    transform:scale(1.1);
    transition: all .5s;
}
.nav-contact{
    padding:2vh 3vw;
    background-color:hsl(51, 100%, 49%);
    color:hsl(0,0%,0%);
    border-radius:20px;
    font-weight:700;
    font-family: 'Fraunces', serif;
    align-self: center;
}
.nav-contact:hover{
    cursor:pointer;
    background-color: hsl(212, 27%, 19%);
    color:hsl(0,100%, 100%);
    transform:scaleX(1.1);
    transition:all .5s;
}
@media screen and (max-width:350px) {
    .head-nav-list{
        padding:3vh 10vw;
        max-width:200px;
    }
}
</style>
<script setup>
import { ref } from "vue";
import DropDownMenu from "./DropDownMenu.vue";

const showMenuBar = ref(false);
const showMenu = ref(false);
const showDropDown = () => {
    if (showMenuBar.value == false) {
        showMenu.value = true;
        showMenuBar.value = true;
    }
    else {
        showMenu.value = false;
        showMenuBar.value = false;
    }
}


</script>

<template>
    <div class="main-header-container">
        <div class="head-logo-container">
            <img src="../assets/images/logo.svg" alt="" class="head-logo">
        </div>
        <div class="head-nav">
            <ul class="head-nav-list">
                <li class="nav">About</li>
                <li class="nav">Services</li>
                <li class="nav">Projects</li>
                <li class="nav-contact" >CONTACT</li>
            </ul>
        </div>
        <div @click="showDropDown()"  class="menu-bar">
            <i v-if="!showMenuBar" class='bx bx-menu'></i>
            <i v-else  class='bx bx-x'></i>
        </div>
        <div class="dropdown">
            <DropDownMenu v-if="showMenu"></DropDownMenu>
        </div>
    </div>
</template>
<style scoped>
.menu-bar {
    font-size:30px;
    display: none;
    color:hsl(0, 100%, 100%);
    
}
.menu-bar:hover{
    transform:scale(0.9);
    transition: all .5s;
}
.dropdown{
    position: absolute;
    top:6vh;
    right:0;
    margin:0 8vw 0 0;
}
.dropdown{
    display:none;
}
.main-header-container{
    display:flex;
    justify-content: space-between;
    padding:0.2vh 3vw 0;
}
.head-logo-container{
    margin:auto 0;
}
.head-nav-list{
    list-style: none;
    color:hsl(0, 100%, 100%);
    display:flex;
    justify-content: space-between;
    gap:3vh;
    font-family: 'Barlow', sans-serif;
}
.nav{
    margin:auto 0;
}
.nav:hover{
    cursor:pointer;
    transform:scale(1.1);
    transition: all .5s;
}
.nav-contact{
    padding:2vh 2vw;
    background-color:hsl(0,100%, 100%);
    color:hsl(0,0%,0%);
    border-radius:20px;
    font-weight:700;
    font-family: 'Fraunces', serif;
}
.nav-contact:hover{
    cursor:pointer;
    background-color: hsla(0, 0%, 100%, 0.384);
    color:hsl(0,100%, 100%);
    transition:all .5s;
}

@media screen and (max-width:850px){
    .head-nav{
        display:none;
    }
    .main-header-container{
        padding:2vh 8vw;
    }
    .dropdown{
        display:block;
    }
    .menu-bar{
        display: block;
    }
}
@media screen and (max-width:400px) {
    .head-logo{
        width:40vw;
    }
}
</style>
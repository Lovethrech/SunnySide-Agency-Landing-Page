<script setup>
import MainHeader from "./components/MainHeader.vue";
import SemiHead from "./components/SemiHead.vue";
import GridUnit from "./components/GridUnit.vue";
import Testimonial from "./components/Testimonial.vue";
import FreeStyleSection from "./components/FreeStyleSection.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <div class="container">
    <div class="head-content">
      <MainHeader></MainHeader>
      <div class="semi-head"><SemiHead></SemiHead></div>
    </div>
    <div class="grid-unit"><GridUnit></GridUnit></div>
    <Testimonial></Testimonial>
    <FreeStyleSection></FreeStyleSection>
    <Footer></Footer>
  </div>
</template>

<style scoped>
.head-content{
  background: url("./assets/images/desktop/image-header.jpg") center center/auto 110vh no-repeat;
  background-size: cover;
}
.semi-head{
  display:flex;
  place-items: center;
  justify-content:center;
  padding: 4vh 0 24vh;
}

@media screen and (max-width: 850px) {
  .head-content{
    background: url("./assets/images/mobile/image-header.jpg") center center/auto 110vh no-repeat;
    background-size: cover;
  }
  .semi-head{
    padding:4vh 8vw 24vh;
  }
}
</style>

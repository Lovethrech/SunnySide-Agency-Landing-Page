<template>
    <div class="freestyle-section-main-container">
        <div class="bottle"></div>
        <div class="orange"></div>
        <div class="cone"></div>
        <div class="sugar-cubes"></div>
    </div>
</template>
<style scoped>
.freestyle-section-main-container{
    width:100%;
    height:400px;
    display:flex;
}
.bottle{
    background: url("../assets/images/desktop/image-gallery-milkbottles.jpg") center/auto no-repeat;
    background-size: cover;
    width:100%;
    height:100%;
}
.orange{
    background: url("../assets/images/desktop/image-gallery-orange.jpg") center/auto no-repeat;
    background-size: cover;
    width:100%;
    height:100%;
}
.cone{
    background: url("../assets/images/desktop/image-gallery-cone.jpg") center/auto no-repeat;
    background-size: cover;
    width:100%;
    height:100%;
}
.sugar-cubes{
    background: url("../assets/images/desktop/image-gallery-sugarcubes.jpg") center/auto no-repeat;
    background-size: cover;
    width:100%;
    height:100%;
}

@media screen and (max-width:850px) {
    .freestyle-section-main-container{
        display:grid;
    }
    .bottle{
        grid-column: 1;
        grid-row:1;
    }
    .orange{
        grid-column: 2;
        grid-row:1;
    }
    .cone{
        grid-column: 1;
        grid-row:2;
    }
    .sugar-cubes{
        grid-column: 2;
        grid-row:2;
    }
}
</style>
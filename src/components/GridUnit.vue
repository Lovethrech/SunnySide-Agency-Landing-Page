<script setup>
import FirstSegment from "./FirstSegment.vue";
import SecondSegment from './SecondSegment.vue';
import ThirdSegment from './ThirdSegment.vue';
</script>

<template>
    <div class="grid-unit-container">
        <div class="first-segment">
            <FirstSegment></FirstSegment>
        </div>

        <div class="second-segment">
            <SecondSegment></SecondSegment>
        </div>

        <div class="third-segment">
            <ThirdSegment></ThirdSegment>
        </div>
    </div>
</template>
<style scoped>
.grid-unit-container{
    margin:0;
    padding:0;
    overflow: hidden;
}




</style>
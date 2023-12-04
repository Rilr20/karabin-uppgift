<script setup>
import HelpButton from './HelpButton.vue';


</script>

<template>
    <header >
        <div class="top-div h-10 flex items-center" >
            <p class="font-bold font-inter text-white ml-48 text-xs">TERRY offert - EN INTERAKTIV OFFERTLÖSNING FRÅN Terry Inc</p>
        </div>
        <div class="bottom-div h-25 pt-6  px-48 flex justify-between">
            <img class="h-10 flex items-center" src="../assets/cloud.png" alt="cloud">
            <help-button />
        </div>
    </header>
</template>
<style scoped>
.top-div {
    background-color: #005874;
}
.bottom-div {
    background-color: #00B5CC;
}
</style>
<script setup>
import HelpButton from './HelpButton.vue';


</script>

<template>
    <header >
        <div class="bg-[#005874] top-div h-10 flex items-center" >
            <p class="font-bold font-inter text-white ml-96 text-xs">TERRY offert - EN INTERAKTIV OFFERTLÖSNING FRÅN Terry Inc</p>
        </div>
        <div class="bg-[#00B5CC]  bottom-div h-25 pt-6  px-96 flex justify-between">
            <img class="h-10 flex items-center" src="../assets/cloud.png" alt="cloud">
            <help-button />
        </div>
    </header>
</template>
<style scoped>

</style>
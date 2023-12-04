<script setup>
import HelpButton from './HelpButton.vue';


</script>

<template>
    <header >
        <div class="bg-[#005874] h-10 flex items-center " >
            <p class="font-bold font-inter text-white md:ml-96 text-xs text-center w-screen md:w-96">TERRY offert - EN INTERAKTIV OFFERTLÖSNING FRÅN Terry Inc</p>
        </div>
        <div class="bg-[#00B5CC] h-16 pt-3 md:h-25 lg:px-96 md:px-20 md:pt-6  flex justify-between ">
            <img class="ml-2 h-10 flex items-center" src="../assets/cloud.png" alt="cloud">
            <help-button />
        </div>
    </header>
</template>
<style scoped>

</style>
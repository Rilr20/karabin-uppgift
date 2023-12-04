<script setup>
import { library } from '@fortawesome/fontawesome-svg-core'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faCircleQuestion } from '@fortawesome/free-solid-svg-icons'

library.add(faCircleQuestion)
</script>
<template>
    <div class="h-10 bg-white xl:px-7 px-4 xl:py-2.5 xl:w-40 xl:h-10 rounded-full flex items-center justify-between text-[#005874]">
        <font-awesome-icon :icon="['fas', 'circle-question']" size="lg" />
        <p class="font-inter font-bold text-xs xl:ml-0 ml-4">Ställ en fråga</p>
    </div>
</template>
<style scoped>

</style>
<script setup>
import { library } from '@fortawesome/fontawesome-svg-core'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faCircleQuestion } from '@fortawesome/free-solid-svg-icons'

library.add(faCircleQuestion)
</script>
<template>
    <div class="h-10 bg-white md:px-7 md:py-2.5 md:w-40 md:h-10 rounded-full flex items-center justify-between text-[#005874]">
        <font-awesome-icon :icon="['fas', 'circle-question']" size="lg" />
        <p class="font-inter font-bold text-xs">Ställ en fråga</p>
    </div>
</template>
<style scoped>

</style>
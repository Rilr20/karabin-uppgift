<script setup>
import { library } from '@fortawesome/fontawesome-svg-core'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faCircleQuestion } from '@fortawesome/free-solid-svg-icons'

library.add(faCircleQuestion)
</script>
<template>
    <div class="bg-white help-button w-29 px-7 py-2.5 w-40 h-10 rounded-full flex items-center justify-between">
        <font-awesome-icon :icon="['fas', 'circle-question']" size="lg" />
        <p class="font-inter font-bold text-xs">Ställ en fråga</p>
    </div>
</template>
<style scoped>
.help-button {
    color: #005874;
}
</style>
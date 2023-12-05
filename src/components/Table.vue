<script setup>

import {defineProps, watch} from 'vue';
const props = defineProps({
    data: Array
});

</script>
<template>
    <table class="table-fixed w-full font-inter md:text-medium text-xs overflow-x"><!--Table-->
        <thead class="text-[#005874] text-center md:h-14 h-20 md:px-0 px-8"><!--Table Header-->
            <th class="md:1/6 w-1/6">Produktnr</th>
            <th class="md:w-40 w-20 pl-4">Benämning</th>
            <th class="md:1/6 w-1/6">Antal</th>
            <th class="md:1/6 w-1/6">Brutto ápris</th>
            <th class="md:1/6 w-1/6">Netto ápris</th>
            <th class="md:1/6 w-1/6">Summa</th>
        </thead>
        <tbody class="text-center sm:overflow-auto">
            <tr class="md:h-14 h-20 md:px-0 px-8 odd:bg-[#F8FDFD] even:bg-white" v-for="row in data">
                <td class="p4 md:1/6 w-1/6">{{ row.id }}</td>
                <td class="p4 text-left md:w-40 w-20 pl-4">{{ row.description }}</td>
                <td class="p4 md:1/6 w-1/6">{{ row.ordered_amount }}</td>
                <td class="p4 md:1/6 w-1/6">{{ row.price }}</td>
                <td class="p4 md:1/6 w-1/6">{{ row.price2 }}</td>
                <td class="p4 md:1/6 w-1/6">{{ row.sum }}</td>
            </tr>

        </tbody>
    </table>
</template>
<style scoped></style>
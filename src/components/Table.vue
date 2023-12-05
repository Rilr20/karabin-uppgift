<script setup>

let data = {
    id: 123452,
    produkt: "Produkt 1 med en längre beskrivning",
    count: 200,
    price: "1 308,00",
    price2: "483,96",
    sum: "193 508,40"
}
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
            <!--Table Row-->
            <tr class="md:h-14 h-20 md:px-0 px-8 odd:bg-[#F8FDFD] even:bg-white">
                <td class="p4 md:1/6 w-1/6">{{ data.id }}</td>
                <td class="p4 text-left md:w-40 w-20 pl-4">Kort titel</td>
                <td class="p4 md:1/6 w-1/6">{{ data.count }}</td>
                <td class="p4 md:1/6 w-1/6">{{ data.price }}</td>
                <td class="p4 2/8">{{ data.price2 }}</td>
                <td class="p4 md:1/6 w-1/6">{{ data.sum }}</td>
            </tr>
            <tr class="md:h-14 h-20 md:px-0 px-8 odd:bg-[#F8FDFD] even:bg-white" v-for="n in 10">
                <td class="p4 md:1/6 w-1/6">{{ data.id }}</td>
                <td class="p4 text-left md:w-40 w-20 pl-4">{{ data.produkt }}</td>
                <td class="p4 md:1/6 w-1/6">{{ data.count }}</td>
                <td class="p4 md:1/6 w-1/6">{{ data.price }}</td>
                <td class="p4 md:1/6 w-1/6">{{ data.price2 }}</td>
                <td class="p4 md:1/6 w-1/6">{{ data.sum }}</td>
            </tr>

        </tbody>
    </table>
</template>
<style scoped></style>
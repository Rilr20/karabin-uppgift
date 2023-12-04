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
    <table class="table-fixed w-fit font-inter"><!--Table-->
        <thead class="text-[#005874] text-center h-14"><!--Table Header-->
            <th class="1/6">Produktnr</th>
            <th class="w-40 pl-4">Benämning</th>
            <th class="1/6">Antal</th>
            <th class="1/6">Brutto ápris</th>
            <th class="1/6">Netto ápris</th>
            <th class="1/6">Summa</th>
        </thead>
        <tbody class="text-center">
            <!--Table Row-->
            <tr class="h-14 odd:bg-[#F8FDFD] even:bg-white">
                <td class="p4 1/6">{{ data.id }}</td>
                <td class="p4 text-left w-40 pl-4">Kort titel</td>
                <td class="p4 1/6">{{ data.count }}</td>
                <td class="p4 1/6">{{ data.price }}</td>
                <td class="p4 2/8">{{ data.price2 }}</td>
                <td class="p4 1/6">{{ data.sum }}</td>
            </tr>
            <tr class="h-14 odd:bg-[#F8FDFD] even:bg-white" v-for="n in 10">
                <td class="p4 1/6">{{ data.id }}</td>
                <td class="p4 text-left w-40 pl-4">{{ data.produkt }}</td>
                <td class="p4 1/6">{{ data.count }}</td>
                <td class="p4 1/6">{{ data.price }}</td>
                <td class="p4 1/6">{{ data.price2 }}</td>
                <td class="p4 1/6">{{ data.sum }}</td>
            </tr>

        </tbody>
    </table>
</template>
<style scoped></style>
<script setup>
import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue'
let data = {
  id: 123452,
  produkt: "produkt 1 med en längre titel",
  count: 200,
  price: "1 308,00",
  price2: "483,96",
  sum: "193 508,40"
}
</script>

<template>
  <Header />
  <div class="font-inter px-96 flex h-screen mt-12 ">
    <div class="flex justify-between w-full h-60"> <!--Two divs section-->
      <div class="bg-white w-1/2 mr-2 bg-[#005874] flex rounded-2xl"> <!--Left div-->
        <div class="w-1/3 pb-4 flex justify-center items-center">
          <img src="../src/assets/items.png" alt="items">
        </div>
        <div class="w-2/3 text-white">
          <p class="text-xs mt-8">Offererad summa:</p>
          <p><span class="text-3xl font-bold">1 736 550 SEK</span> exkl. moms</p>
          <div class="grid grid-rows-2 grid-flow-col gap-4 mt-8 text-xs"> <!--grid-->
            <div>
              <p class="font-bold">Offertnummer</p>
              <p>8971235</p>
            </div>

            <div>
              <p class="font-bold">Vår referens</p>
              <p>Brian Kilback</p>
            </div>
            <div>
              <p class="font-bold">Offertdatum</p>
              <p>2023-12-04</p>
            </div>
            <div>
              <p class="font-bold">Er referens</p>
              <p>Marcus Andersson</p>
            </div>
          </div>
        </div>
      </div>
      <div class="w-1/2 ml-2 bg-gradient-to-r to-[#00B5CC] from-[#005874] rounded-2xl"> <!--Right div-->

        <!-- <div class=" h-full">
          text2
        </div> -->
      </div>
    </div>
    <div class=""> <!--Table section-->
      <div class=""><!--Table-->

      </div>
      <div class=""><!--Customer Info section-->

      </div>
      <div class=""><!--Information-->

      </div>
    </div>
  </div>
</template>

<style scoped></style>

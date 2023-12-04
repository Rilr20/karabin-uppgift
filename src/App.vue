<script setup>
import Header from './components/Header.vue'
import Table from './components/Table.vue'
import { library } from '@fortawesome/fontawesome-svg-core'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faFilePdf } from '@fortawesome/free-regular-svg-icons'

library.add(faFilePdf)
</script>

<template>
  <Header />
  <div class="font-inter md:px-96 h-screen mt-12 md:overflow-x-auto overflow-x-hidden">
    <div class="md:flex justify-between w-full h-60"> <!--Two divs section-->
      <div class="md:w-1/2 w-fill md:mr-2 bg-[#005874] flex rounded-2xl md:mb-0 mb-8"> <!--Left div-->
        <div class="md:w-1/3 pb-4 w-0 md:flex justify-center items-center invisible md:visible">
          <img class="" src="../src/assets/items.png" alt="items">
        </div>
        <div class="md:w-2/3 w-fill md:px-0 px-8 md:pb-o pb-4 text-white">
          <p class="text-xs mt-8">Offererad summa:</p>
          <p><span class="text-3xl font-bold">1 736 550 SEK</span> exkl. moms</p>
          <div class="grid grid-rows-2 grid-flow-col gap-4 mt-8 text-xs"> <!--grid?-->
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
      <div class="md:w-1/2 w-fill md:ml-2 bg-gradient-to-r to-[#00B5CC] from-[#005874] rounded-2xl text-white text-xs flex">
        <!--Right div-->
        <div class="p-8 font-medium md:w-4/6 w-fill"> <!--Text-->
          <p>Hej Brian,</p>
          <br> <br>
          <p class="md:mr-0 mr-16"><!--När texten är längre än "Tack för Er förfrågan. Om du har några frågor s" då blir det en overflow av någon anledning-->
            Tack för Er förfrågan. Om du har några frågor så kan du nå mig på 0707 - 54 54 54 eller via
            kontaktinformationen direkt här på sidan
          </p>
          <br> <br>
          <p>Mvh</p>
          <p>Julius Davis</p>
          <p>Säljare Terry Inc.</p>
        </div>
        <div class="w-0 md:w-2/6 bg-color[#ff22ff] md:static invisible md:visible"><!--Image-->
          <img class="relative rounded-2xl bottom-18 left-13 " style="bottom:18px;left:13px;" src="../src/assets/man.png"
            alt="man">
        </div>
      </div>
    </div>

    <div class="md:flex mt-6"> <!--Table section-->
      <div class="md:w-4/6 w-fill md:mr-2 rounded-2xl"> <!--Left -->
        <div class="w-fit bg-white rounded-2xl p-8 md:mt-0 mt-72">
          <Table />
        </div>
        <div class="bg-white mt-8 rounded-2xl p-8 text-[#005874]">
          <h3 class="text-base mb-4 mt-2 font-bold">Information</h3>
          <p class="text-xs">Quis tenetur ratione. Neque molestias doloribus suscipit. 
            Dolor quisquam pariatur minima voluptatem. 
            Natus eligendi nostrum odit excepturi saepe alias saepe. 
            Vero eum illo ad hic consequuntur beatae.
          </p>
          <h3 class="text-base mb-4 mt-4 font-bold">Frakt</h3>
          <p class="text-xs">Observera att frakt, pall och emballage inte ingår i priset och tillkommer. Leveranstiden för ej lagerförda material är 6-8 veckor. 
            Vi följer gällande standarder. Offerten är giltig i 30 dagar och priset avser endast de artiklar som anges i offerten. 
            Priserna är baserade på en överenskommen rabatt gentemot bruttoprislistan. 
            Var vänlig kontrollera offerten noggrant då Watt inte tar ansvar för eventuella fel i produktbeskrivningen.
          </p>
        </div>
      </div>
      <div class="md:w-2/6 w-fill h-fit md:ml-2"><!--Right-->
        <div class="bg-white w-fill p-8 rounded-2xl">


          <div class="grid grid-rows-3 grid-flow-col gap-1  text-xs text-[#005874] "><!--Shipping Info section-->
            <div class="my-2">
              <p class="text-sm font-bold">Kundnummer</p>
              <p>3320</p>
            </div>
            <div class="my-2">
              <p class="text-sm font-bold">Er Order</p>
              <p>Tideräkningsgatan</p>

            </div>
            <div class="my-2">
              <p class="text-sm font-bold">Leveransvilkor</p>
              <p>Fritt vårt lager CPT</p>
            </div>
            <div class="my-2">
              <p class="text-sm font-bold">Betalningsvilkor</p>
              <p>30 dagar</p>

            </div>
            <div class="my-2">
              <p class="text-sm font-bold">Godsmärke</p>
              <p>Tideräkningsgatan</p>
            </div>
          </div>
        </div>

        <div class="bg-[#00B5CC] text-white my-4 rounded-2xl h-14 flex justify-center items-center"> <font-awesome-icon :icon="['far', 'file-pdf']" /> Ladda ner PDF</div>
        <div class="bg-[#005874] text-white my-4 rounded-2xl h-14 flex justify-center items-center">Godkänn offert</div>
        <div class="bg-[#fff] text-[#F16A80] my-4 rounded-2xl h-14 flex justify-center items-center">Neka offert</div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>

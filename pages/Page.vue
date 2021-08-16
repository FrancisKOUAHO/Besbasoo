<template>
  <div class="bg-gray-200">
    <Nav class="ma-0" />
    <Slider />
    <div class=" py-5 px-10 flex justify-between ">
      <div class="text-xl font-bold font-rambla">
        Les offres du moment
      </div>
    </div>
    <div class="flex-auto md:flex justify-center my-10 flex-warp w-full">
      <Cardslides v-for="i in 4" v-bind:key="i" />
    </div>

    <div
      class="w-full relative bg-gradient-to-r  from-gray-900 via-gray-900 to-gray-900"
      style=" height: 494px;"
    >
      <!-- <img
        class="  "
        style="width: 792px; height: 494px;"
        src="../components/images/image.png"
      /> -->
      <div class="absolute right-5 top-5 items-end flex">
        <p class="text-4xl font-bold text-white">Besbasoo</p>
        <p class="text-2xl pl-1 italic  font-italic text-white">watch</p>
      </div>
      <div
        class="md:w-1/3 w-1/2 absolute text-2xl md:text-4xl md:font-bold text-white left-10  top-20 md:left-10 md:top-20 "
      >
        <p>
          Profitez de l’offre de lancement et bénéficiez de 3 mois gratuits*
          puis de seulement 8,99€/mois
        </p>
      </div>
      <button
        class="w-56 h-14 bottom-10 left-5 md:left-10 absolute bg-yellow-500 text-3xl text-white text-center rounded-md"
      >
        En savoir plus
      </button>
    </div>
    <br />
    <br />
    <div class="flex justify-between  py-5 px-10">
      <div class="text-xl font-bold font-rambla">
        Sélectionner spécialement pour vous
      </div>
    </div>
    <div class="flex-warp md:px-5 justify-between text-center py-10">
      <SecondSlider v-for="i in 5" v-bind:key="i" />
    </div>

    <div class="flex justify-between  py-5 px-10">
      <div class="text-xl font-bold font-rambla">
        Catégorie
      </div>
    </div>
    <div class="flex-warp px-5 justify-between text-center py-10">
      <SmallCard v-for="i in 10" v-bind:key="i" />
    </div>

    <div class=" flex justify-center text-xl w-full   mb-10  text-center py-10 px-3 font-rambla">
      <div>
         <img class="ml-20" src="../components/images/2-arraow.png">
          <a href="#" class="my-3 duration-700 fontrambla">
            RETOURNER EN HAUT
          </a>
      </div>
    </div>

    <Footer class="ma-0" />
  </div>
</template>
<script>
import Slider from "../components/page2/Slider.vue";
import Cardslides from "../components/page2/Card_Slide.vue";
import SmallCard from "../components/page2/SmallCard.vue";
import SecondSlider from "../components/page2/SecondSlider.vue";
export default {
  components: { Cardslides, Slider, SecondSlider, SmallCard }
};
</script>

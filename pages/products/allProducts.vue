<template>
  <div>
    <div class="flex justify-between  py-5 px-3">
      <div class="text-xl font-bold font-rambla">
        Résultats (518)
      </div>
      <div class="text-xl font-bold font-rambla">
        <button class="pa-2 px-5 border-2 border-gray-500">Trier par</button>
      </div>
    </div>
    <div v-for="(a,index) in array"  class="flex-auto md:flex flex-warp w-full">
      <Card /> <Card /><Card /><Card /> <Card />
    </div>
    <Pagination class="py-10 text-right mobile-view-pag" />
    <div class=" flex justify-center text-xl w-full   mb-10  text-center py-10 px-3 font-rambla">
      <div>

          <a href="#" class="my-3 duration-700 fontrambla">
            <img class="ml-20" src="~/assets/images/arraow.png" alt="arraow" width="30">
            RETOURNER EN HAUT
          </a>
      </div>
    </div>
  </div>
</template>
<script>
  import Card from '../../components/page1/Card.vue'
  import Pagination from '../../components/page1/Pagination.vue'
  export default {
     components:{Card,Pagination},
     data(){
       return{
          array: [1,2,3,4,5],
       }
     },
    head() {
      return {
        title: 'allProducts | Besbasoo',
        meta: [
          {
            hid: 'description',
            name: 'description',
            content: 'Ma description personnalisée'
          }
        ]
      }
    }

  }
</script>
<style scoped>
   .fontrambla{
     font-family: Rambla,serif;
   }


  @media only screen and (max-width: 658px) {
    .mobile-view-pag{
      text-align: center;
    }
  }



</style>

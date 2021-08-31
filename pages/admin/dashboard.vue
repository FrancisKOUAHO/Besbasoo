<template>
  <div>
    <h1 class='text-2xl text-black-600 font-bold'>Dashboard</h1>
    <div class='mt-2.5 w-full flex list-total-savings'>
      <div class='flex flex-row w-full mx-2 bg-white shadow-lg p-4 items-center justify-center text-left rounded-lg'>
        <div class='w-1/5'>
          <img src="@/assets/images/icon-total-sales.png">
        </div>
        <div class='w-4/5 ml-6'>
          <h2 class='text-xl text-gray-400'>
            Gain total
          </h2>
          <span class='text-2xl text-black-600 font-bold'>19,626,058.20€</span>
        </div>
      </div>
      <div class='flex flex-row w-full mx-2 bg-white shadow-lg p-4 items-center justify-center text-left rounded-lg'>
        <div class='w-1/5'>
          <img src="@/assets/images/icon-total-orders.png">
        </div>
        <div class='w-4/5 ml-6'>
          <h2 class='text-xl text-gray-400'>
            Nombre de ventes
          </h2>
          <span class='text-2xl text-black-600 font-bold'>3290</span>
        </div>
      </div>
      <div class='flex flex-row w-full mx-2 bg-white shadow-lg p-4 items-center justify-center text-left rounded-lg'>
        <div class='w-1/5'>
          <img src="@/assets/images/icon-total-products.png">
        </div>
        <div class='w-4/5 ml-6'>
          <h2 class='text-xl text-gray-400'>
            Nombre de produits
          </h2>
          <span class='text-2xl text-black-600 font-bold'>322</span>
        </div>
      </div>
    </div>
    <Table />
  </div>
</template>

<script>
import AdminNavbar from "@/components/Navbars/AdminNavbar";
import Table from "@/components/admin/Table";

export default {
  name: "dashboard",
  layout: 'admin',
  components: {AdminNavbar, Table}
}
</script>

<style scoped>


</style>

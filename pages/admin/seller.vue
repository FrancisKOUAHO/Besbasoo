<template>
  <div class="premiere-div">
    <h1>{{titlePage}}</h1>
    <div class="deuxieme-div">
      <h2>{{titlePage}}</h2>
    </div>
  </div>
</template>

<script>
import AdminNavbar from "@/components/Navbars/AdminNavbar";

export default {
  name: "seller",
  layout: 'admin',
  data() {
    return {
      titlePage: 'Vendeurs'
    }
  },
  components: {AdminNavbar}
}
</script>

<style lang="scss">
  .premiere-div{
    background: red;
    h1 {
      font-size: 5rem;
    }
  }

  .deuxieme-div {
    background: green;
    h2 {
      font-size: 10rem;
    }
  }
</style>

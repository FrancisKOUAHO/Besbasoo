<template>
  <div class="bg-gray-100 font-family-karla flex">
    <aside class="relative bg-sidebar h-screen w-64 hidden sm:block shadow-xl">
      <div class="p-6">
        <router-link :to="{name: 'Accueil'}">
          <!--          <img src="@/assets/image/logo/Logo_Skyplus.svg"-->
          <!--               class="text-white text-3xl font-semibold uppercase hover:text-gray-300"/>-->
          <button
            class="w-full bg-white cta-btn font-semibold py-2 mt-5 rounded-br-lg rounded-bl-lg rounded-tr-lg shadow-lg hover:shadow-xl hover:bg-gray-300 flex items-center justify-center">
            Rôle: Administrateur
          </button>
        </router-link>
      </div>
      <nav class="text-white text-base font-semibold pt-3">
        <router-link to="#" class="flex items-center active-nav-link text-white py-4 pl-6 nav-item">
          <i class="fas fa-tachometer-alt mr-3"></i>
          Tableau de bord
        </router-link>
        <router-link to="#"
                     class="flex items-center text-white opacity-75 hover:opacity-100 py-4 pl-6 nav-item">
          <i class="fas fa-sticky-note mr-3"></i>
          Produits
        </router-link>
        <router-link to="#"
                     class="flex items-center text-white opacity-75 hover:opacity-100 py-4 pl-6 nav-item">
          <i class="fas fa-sticky-note mr-3"></i>
          Commandes
        </router-link>
        <a href="http://invoice.skyplus.fr"
           class="flex items-center text-white opacity-75 hover:opacity-100 py-4 pl-6 nav-item">
          <i class="fas fa-sticky-note mr-3"></i>
          Transactions
        </a>
        <router-link to="#"
                     class="flex items-center text-white opacity-75 hover:opacity-100 py-4 pl-6 nav-item">
          <i class="fas fa-sticky-note mr-3"></i>
          Clients
        </router-link>
        <router-link to="#"
                     class="flex items-center text-white opacity-75 hover:opacity-100 py-4 pl-6 nav-item">
          <i class="fas fa-table mr-3"></i>
          Vendeurs
        </router-link>
        <router-link to="#"
                     class="flex items-center text-white opacity-75 hover:opacity-100 py-4 pl-6 nav-item">
          <i class="fas fa-calendar mr-3"></i>
          Paramètre
        </router-link>
      </nav>
    </aside>

    <div class="w-full flex flex-col h-screen overflow-y-hidden">
      <!-- Desktop Header -->
      <header class="w-full items-center bg-white py-2 px-6 hidden sm:flex">
        <div class="w-1/2"></div>
        <div class="relative w-1/2 flex justify-end">
          <div class="flex">
            <div class="relative">
              <button
                class="rounded-full overflow-hidden border-2  w-10 h-10 flex justify-center items-center | hover:border-white focus:outline-none focus:border-white"
                @click="isOpen1 = true"
              >
              <img src="/logo-1.png" alt="User's avatar">
              </button>
              <div v-if="isOpen1" class="fixed inset-0 w-full h-screen z-20 bg-black opacity-25"
                   @click="isOpen1 = false"></div>
              <div v-if="isOpen1" class="absolute z-30 right-0 mt-2" :class="{'hidden': !isOpen1}">
                <div class="bg-white rounded-lg shadow-lg py-2 w-48">
                  <ul>
                    <li
                      class="block color-text text-purple-600 font-semibold px-4 py-2"><span>Profil</span>
                    </li>
                    <li
                      class="block color-text text-purple-600 font-semibold px-4 py-2"><span>Paramètres</span>
                    </li>
                    <li
                        class="block color-text text-purple-600 font-semibold px-4 py-2"><span>Se déconnecter</span>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
        </div>
      </header>

      <div class="w-full overflow-x-hidden border-t flex flex-col">
        <main class="w-full flex-grow p-6">
          <h1 class="text-3xl text-black pb-6">Tableau de bord
          </h1>
          <nuxt/>
        </main>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "admin",
  data() {
    return {
      isOpen1: false,
      isOpen2: true,
    }
  }
}
</script>

<style scoped>
.font-family-karla {
  font-family: Rambla,serif;
}
.bg-sidebar {
  background: #093d8b;
}
.cta-btn {
  color: #093d8b;
}
.active-nav-link {
  background: #093d8b;
}
.nav-item:hover {
  background: #093d8b;
}
.color-text {
  color: black !important;
}
.color-text:hover {
  color: #093d8b !important;
}

</style>

<template>
    <div>
        <h1 class='text-2xl text-black-600 font-bold mb-5'>Détails de la commande N°598764</h1>
        <div class="bg-white rounded-lg w-full p-6 shadow-lg">
            <div class="flex justify-between pb-6">
              <div class="flex flex-row items-center">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M20 20h-4v-4h4v4zm-6-10h-4v4h4v-4zm6 0h-4v4h4v-4zm-12 6h-4v4h4v-4zm6 0h-4v4h4v-4zm-6-6h-4v4h4v-4zm16-8v22h-24v-22h3v1c0 1.103.897 2 2 2s2-.897 2-2v-1h10v1c0 1.103.897 2 2 2s2-.897 2-2v-1h3zm-2 6h-20v14h20v-14zm-2-7c0-.552-.447-1-1-1s-1 .448-1 1v2c0 .552.447 1 1 1s1-.448 1-1v-2zm-14 2c0 .552-.447 1-1 1s-1-.448-1-1v-2c0-.552.447-1 1-1s1 .448 1 1v2z"/></svg>
                <span class="ml-4 text-lg font-bold text-black-600 text-left">
                  Samedi 11 Septembre, 2021, 16:34  
                </span>
              </div>
                <div class="flex justify-center">

                    <div class="relative inline-block text-left dropdown ml-1">
                        <span class="rounded-md shadow-sm"
                        ><button class="inline-flex justify-center w-full px-4 py-2 text-sm font-medium leading-5 text-gray-700 transition duration-150 ease-in-out bg-white border border-gray-300 rounded-md hover:text-gray-500 focus:outline-none focus:border-blue-300 focus:shadow-outline-blue active:bg-gray-50 active:text-gray-800" 
                        type="button" aria-haspopup="true" aria-expanded="true" aria-controls="headlessui-menu-items-117">
                            <span class="text-gray-500 font-bold">Changer de Statut</span>
                            <svg class="w-5 h-5 ml-2 -mr-1" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
                            </button
                        ></span>
                        <div class="opacity-0 invisible dropdown-menu transition-all duration-300 transform origin-top-right -translate-y-2 scale-95">
                        <div class="absolute right-0 w-56 mt-2 origin-top-right bg-white border border-gray-200 divide-y divide-gray-100 rounded-md shadow-lg outline-none" aria-labelledby="headlessui-menu-button-1" id="headlessui-menu-items-117" role="menu">
                            <div class="py-1">
                            <a href="javascript:void(0)" tabindex="0" class="text-gray-700 flex justify-between w-full px-4 py-2 text-sm leading-5 text-left"  role="menuitem" >Délivré</a>
                            <a href="javascript:void(0)" tabindex="1" class="text-gray-700 flex justify-between w-full px-4 py-2 text-sm leading-5 text-left"  role="menuitem" >En transit</a>
                            <span role="menuitem" tabindex="-1" class="flex justify-between w-full px-4 py-2 text-sm leading-5 text-left text-gray-700 cursor-not-allowed opacity-50" aria-disabled="true">En traitement</span>
                            <a href="javascript:void(0)" tabindex="2" class="text-gray-700 flex justify-between w-full px-4 py-2 text-sm leading-5 text-left" role="menuitem" >Annulé</a></div>
                        </div>
                        </div>
                    </div>
                    <button class="ml-2 text-gray-500 font-bold rounded-md border px-2">
                        Enregistrer
                    </button>
                    <button class="ml-2 bg-gray-500 rounded-md border px-2">
                        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24"><path fill="white" d="M24 5h-4v-5h-16v5h-4v13h4v6h9.519c2.947 0 6.029-3.577 6.434-6h4.047v-13zm-18-3h12v3h-12v-3zm8.691 16.648s1.469 3.352-2 3.352h-6.691v-8h12v2.648c0 3.594-3.309 2-3.309 2zm6.809-10.648c-.276 0-.5-.224-.5-.5s.224-.5.5-.5.5.224.5.5-.224.5-.5.5zm-5.5 9h-8v-1h8v1zm-3 1h-5v1h5v-1z"/></svg>
                    </button>
                </div>
            </div>
            <div class="w-full pt-6 flex flex-row justify-between items-center border-t">
                <div class='flex flex-row items-start justify-center text-left'>
                  <div class='w-14'>
                    <img src="@/assets/images/icon-customer.png">
                  </div>
                  <div class='flex flex-col ml-6'>
                    <h3 class="text-lg font-bold text-black-600">Acheteur</h3>
                    <span class="text-md text-gray-500">ESHAL Rosas</span>
                    <span class="text-md text-gray-500">ESHAL.Rosas@gmail.com</span>
                    <span class="text-md text-gray-500">(+33) 06 45 98 74 12</span>
                    <router-link :to="{name: 'admin-clientProfil'}"
                      class="text-md text-blue-400 hover:underline">
                            Voir profil
                    </router-link>
                  </div>
                </div>
                <div class='flex flex-row items-start justify-center text-left'>
                  <div class='w-14'>
                    <img src="@/assets/images/icon-shipping.png">
                  </div>
                  <div class='flex flex-col ml-6'>
                    <h3 class="text-lg font-bold text-black-600">Moyens</h3>
                    <span class="text-md text-gray-500">Transporteur : Chronopost</span>
                    <span class="text-md text-gray-500">Moyen de paiement : Paypal</span>
                    <span class="text-md text-gray-500">Statut : En transit</span>
                    <a href="path_to_file" download="proposed_file_name" class="text-md text-blue-400 hover:underline">Télécharger</a>
                  </div>
                </div>
                <div class='flex flex-row items-start justify-center text-left'>
                  <div class='w-14'>
                    <img src="@/assets/images/icon-adress.png">
                  </div>
                  <div class='flex flex-col ml-6'>
                    <h3 class="text-lg font-bold text-black-600">Adresse de livraison</h3>
                    <span class="text-md text-gray-500">Ville : Pontault-Combault</span>
                    <span class="text-md text-gray-500">Code postal : 77340</span>
                    <span class="text-md text-gray-500">Adresse : 24 Avenue de la République</span>
                    <a href="https://www.google.fr/maps/place/5+Av.+George+V,+75008+Paris/@48.8655941,2.2989462,17z/data=!3m1!4b1!4m9!1m2!2m1!1s5+avenue+George+V!3m5!1s0x47e66fdd65c4f269:0x7090ed627190ef07!8m2!3d48.8655906!4d2.3011349!15sChE1IGF2ZW51ZSBHZW9yZ2UgVpIBEGdlb2NvZGVkX2FkZHJlc3M" target="_blank" class="text-md text-blue-400 hover:underline">Voir sur la carte</a>
                  </div>
                </div>
            </div>
            <div class="w-full flex flex-row justify-between mt-6">
                <RecapShipping class="mr-2"/>
                <div class="flex flex-col w-2/6 ml-2">
                  <div class="flex flex-col p-4 rounded-lg border bg-gray-100">
                    <h3 class="text-lg font-bold text-black-600">Information de paiement</h3>
                    <span class="text-md text-gray-500">Master Carte **** **** **** 4975</span>
                    <span class="text-md text-gray-500">Nom de la carte : MME ROSAS ESHAL</span>
                    <span class="text-md text-gray-500">Numéro de téléphone : (+33) 06 45 98 74 12</span>
                  </div>
                  <label class="text-md text-gray-500 mt-6">Notes</label>
                  <textarea class="border rounded-lg" rows="4">
                  </textarea>
                  <button type="button" class="py-2 bg-blue-600 rounded-md text-white outline-none focus:ring-4 transform active:scale-x-75 transition-transform mt-4 text-center">
                      <span class="text-xl">Enregistrer les modifications</span>
                  </button>
                </div>
            </div>
        </div>

    </div>
</template>

<script>
import AdminNavbar from "@/components/Navbars/AdminNavbar";
import Product from "@/components/admin/Product";
import RecapShipping from "@/components/admin/RecapShipping";

export default {
  name: "products",
  layout: 'admin',
  components: {AdminNavbar, Product, RecapShipping}
}
</script>

<style scoped>
.dropdown:focus-within .dropdown-menu {
  opacity:1;
  transform: translate(0) scale(1);
  visibility: visible;
}
input {
    padding-left: 0.75em;
}

/* input::placeholder {
    font-size; 
} */
</style>

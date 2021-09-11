<template>
    <div>
        <div class="flex justify-between items-center mb-5">
            <h1 class='text-2xl text-black-600 font-bold'>Clients</h1>
        </div>
        <div class="banner bg-white rounded-lg w-full px-6 pb-6 pt-40 shadow-lg mb-5">
            <div class="flex items-end justify-between pb-6">
                <div class="flex flex-row items-end">
                    <img class="w-40 border-2 border-white rounded-md" src="https://oasys.ch/wp-content/uploads/2019/03/photo-avatar-profil.png"/>
                    <div class="flex flex-col ml-6">
                        <h3 class="text-2xl font-bold text-black-600">ESHAL Rosas</h3>
                        <h3 class="text-lg text-gray-500">24 Avenue de la République, 77340 Pontault-Combault</h3>
                    </div>
                </div>
                <div class="flex justify-center">
                    <div class="relative inline-block text-left dropdown mx-1">
                        <span class="rounded-md shadow-sm"
                        ><button class="inline-flex justify-center w-full px-4 py-2 text-sm font-medium leading-5 text-gray-700 transition duration-150 ease-in-out bg-white border border-gray-300 rounded-md hover:text-gray-500 focus:outline-none focus:border-blue-300 focus:shadow-outline-blue active:bg-gray-50 active:text-gray-800" 
                        type="button" aria-haspopup="true" aria-expanded="true" aria-controls="headlessui-menu-items-117">
                            <span class="text-gray-500 font-bold">Actions</span>
                            <svg class="w-5 h-5 ml-2 -mr-1" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
                            </button
                        ></span>
                        <div class="opacity-0 invisible dropdown-menu transition-all duration-300 transform origin-top-right -translate-y-2 scale-95">
                        <div class="absolute right-0 w-56 mt-2 origin-top-right bg-white border border-gray-200 divide-y divide-gray-100 rounded-md shadow-lg outline-none" aria-labelledby="headlessui-menu-button-1" id="headlessui-menu-items-117" role="menu">
                            <div class="py-1">
                            <a href="javascript:void(0)" tabindex="0" class="text-gray-700 flex justify-between w-full px-4 py-2 text-sm leading-5 text-left"  role="menuitem" >Afficher par 8</a>
                            <a href="javascript:void(0)" tabindex="1" class="text-gray-700 flex justify-between w-full px-4 py-2 text-sm leading-5 text-left"  role="menuitem" >Afficher par 16</a>
                            <span role="menuitem" tabindex="-1" class="flex justify-between w-full px-4 py-2 text-sm leading-5 text-left text-gray-700 cursor-not-allowed opacity-50" aria-disabled="true">Afficher par 32</span>
                            <a href="javascript:void(0)" tabindex="2" class="text-gray-700 flex justify-between w-full px-4 py-2 text-sm leading-5 text-left" role="menuitem" >Afficher tout</a></div>
                        </div>
                        </div>
                    </div>

                    <div class="relative inline-block text-left dropdown ml-1">
                        <span class="rounded-md shadow-sm"
                        ><button class="inline-flex justify-center w-full px-4 py-2 text-sm font-medium leading-5 text-gray-700 transition duration-150 ease-in-out bg-white border border-gray-300 rounded-md hover:text-gray-500 focus:outline-none focus:border-blue-300 focus:shadow-outline-blue active:bg-gray-50 active:text-gray-800" 
                        type="button" aria-haspopup="true" aria-expanded="true" aria-controls="headlessui-menu-items-117">
                            <span class="text-gray-500 font-bold">Voir les statistiques</span>
                            <svg xmlns="http://www.w3.org/2000/svg" class="ml-2" width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0c-6.627 0-12 5.373-12 12s5.373 12 12 12 12-5.373 12-12-5.373-12-12-12zm1 16.057v-3.057h2.994c-.059 1.143-.212 2.24-.456 3.279-.823-.12-1.674-.188-2.538-.222zm1.957 2.162c-.499 1.33-1.159 2.497-1.957 3.456v-3.62c.666.028 1.319.081 1.957.164zm-1.957-7.219v-3.015c.868-.034 1.721-.103 2.548-.224.238 1.027.389 2.111.446 3.239h-2.994zm0-5.014v-3.661c.806.969 1.471 2.15 1.971 3.496-.642.084-1.3.137-1.971.165zm2.703-3.267c1.237.496 2.354 1.228 3.29 2.146-.642.234-1.311.442-2.019.607-.344-.992-.775-1.91-1.271-2.753zm-7.241 13.56c-.244-1.039-.398-2.136-.456-3.279h2.994v3.057c-.865.034-1.714.102-2.538.222zm2.538 1.776v3.62c-.798-.959-1.458-2.126-1.957-3.456.638-.083 1.291-.136 1.957-.164zm-2.994-7.055c.057-1.128.207-2.212.446-3.239.827.121 1.68.19 2.548.224v3.015h-2.994zm1.024-5.179c.5-1.346 1.165-2.527 1.97-3.496v3.661c-.671-.028-1.329-.081-1.97-.165zm-2.005-.35c-.708-.165-1.377-.373-2.018-.607.937-.918 2.053-1.65 3.29-2.146-.496.844-.927 1.762-1.272 2.753zm-.549 1.918c-.264 1.151-.434 2.36-.492 3.611h-3.933c.165-1.658.739-3.197 1.617-4.518.88.361 1.816.67 2.808.907zm.009 9.262c-.988.236-1.92.542-2.797.9-.89-1.328-1.471-2.879-1.637-4.551h3.934c.058 1.265.231 2.488.5 3.651zm.553 1.917c.342.976.768 1.881 1.257 2.712-1.223-.49-2.326-1.211-3.256-2.115.636-.229 1.299-.435 1.999-.597zm9.924 0c.7.163 1.362.367 1.999.597-.931.903-2.034 1.625-3.257 2.116.489-.832.915-1.737 1.258-2.713zm.553-1.917c.27-1.163.442-2.386.501-3.651h3.934c-.167 1.672-.748 3.223-1.638 4.551-.877-.358-1.81-.664-2.797-.9zm.501-5.651c-.058-1.251-.229-2.46-.492-3.611.992-.237 1.929-.546 2.809-.907.877 1.321 1.451 2.86 1.616 4.518h-3.933z"/></svg>
                            </button
                        ></span>
                        <div class="opacity-0 invisible dropdown-menu transition-all duration-300 transform origin-top-right -translate-y-2 scale-95">
                        <div class="absolute right-0 w-56 mt-2 origin-top-right bg-white border border-gray-200 divide-y divide-gray-100 rounded-md shadow-lg outline-none" aria-labelledby="headlessui-menu-button-1" id="headlessui-menu-items-117" role="menu">
                            <div class="py-1">
                            <span role="menuitem" tabindex="-1" class="flex justify-between w-full px-4 py-2 text-sm leading-5 text-left text-gray-700 cursor-not-allowed opacity-50" aria-disabled="true">Les plus récents</span>
                            <a href="javascript:void(0)" tabindex="2" class="text-gray-700 flex justify-between w-full px-4 py-2 text-sm leading-5 text-left" role="menuitem" >Les plus anciens</a></div>
                        </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="w-full pt-6 border-t flex flex-row items-start justify-between">
                <div class="flex flex-col border w-2/12 rounded-md p-4">
                    <div>
                        <h3 class="text-lg text-gray-500">Total acheté</h3>
                        <span class="text-2xl font-bold text-green-500">15</span>
                    </div>
                    <div>
                        <h3 class="text-lg text-gray-500">Dépensé</h3>
                        <span class="text-2xl font-bold text-green-500">$287,69</span>
                    </div>
                </div>
                <div class="flex flex-col w-1/4 ml-6">
                    <h3 class="text-2xl font-bold text-black-600">Contact</h3>
                    <span class="text-lg text-gray-500">ESHAL.Rosas@gmail.com</span>
                    <span class="text-lg text-gray-500">(+33) 06 45 98 74 12 54</span>
                </div>
                <div class="flex flex-col w-1/4">
                    <h3 class="text-2xl font-bold text-black-600">Adresse de livraison</h3>
                    <span class="text-lg text-gray-500">Pays : France</span>
                    <span class="text-lg text-gray-500">Adresse  : 24 Avenue de la République</span>
                    <span class="text-lg text-gray-500">Ville : Pontault-Combault</span>
                    <span class="text-lg text-gray-500">Code postal : 77340</span>
                </div>
                <div class="flex flex-col w-1/4">
                    <h3 class="text-2xl font-bold text-black-600">Adresse de facturation</h3>
                    <span class="text-lg text-gray-500">Pays : France</span>
                    <span class="text-lg text-gray-500">Adresse  : 24 Avenue de la République</span>
                    <span class="text-lg text-gray-500">Ville : Pontault-Combault</span>
                    <span class="text-lg text-gray-500">Code postal : 77340</span>
                </div>
            </div>
        </div>

        <div class="bg-white rounded-lg w-full p-6 shadow-lg">
            <h2 class='text-2xl text-black-600 font-bold'>Produits achetés</h2>
            <div class="w-full pt-6 grid grid-flow-col grid-rows-2 grid-cols-4 gap-3">
                <ClientProduct />
                <ClientProduct />
                <ClientProduct />
                <ClientProduct />
                <ClientProduct />
                <ClientProduct />
                <ClientProduct />
                <ClientProduct />
            </div>
            <Pagination class="mt-7" />
        </div>
    </div>
</template>

<script>
import AdminNavbar from "@/components/Navbars/AdminNavbar";
import ClientProduct from "@/components/admin/ClientProduct";
import Pagination from "@/components/tools/pagination";

export default {
  name: "sellerProfil",
  layout: 'admin',
  components: {AdminNavbar, ClientProduct, Pagination}
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
.banner {
    background-image: url(@/assets/images/banniere.jpg);
    background-position: center -29em;
    background-repeat: no-repeat;
    background-size: cover;
}
</style>

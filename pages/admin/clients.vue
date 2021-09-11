<template>
    <div>
        <h1 class='text-2xl text-black-600 font-bold mb-5'>Clients</h1>
        <div class="bg-white rounded-lg w-full p-6 shadow-lg">
            <div class="flex justify-between pb-6">
                <input type="text" size="60" placeholder="Rechercher un client" class="border rounded-md">
                <div class="flex justify-center">

                    <div class="relative inline-block text-left dropdown mx-1">
                        <span class="rounded-md shadow-sm"
                        ><button class="inline-flex justify-center w-full px-4 py-2 text-sm font-medium leading-5 text-gray-700 transition duration-150 ease-in-out bg-white border border-gray-300 rounded-md hover:text-gray-500 focus:outline-none focus:border-blue-300 focus:shadow-outline-blue active:bg-gray-50 active:text-gray-800" 
                        type="button" aria-haspopup="true" aria-expanded="true" aria-controls="headlessui-menu-items-117">
                            <span class="text-gray-500 font-bold">Affichage</span>
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
                            <span class="text-gray-500 font-bold">Date</span>
                            <svg class="w-5 h-5 ml-2 -mr-1" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
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
            <div class="w-full pt-6 grid grid-flow-col grid-rows-2 grid-cols-4 gap-3 border-t">
                <Client />
                <Client />
                <Client />
                <Client />
                <Client />
                <Client />
                <Client />
                <Client />
            </div>
        </div>
        <Pagination class="mt-7" />
    </div>
</template>

<script>
import AdminNavbar from "@/components/Navbars/AdminNavbar";
import Client from "@/components/admin/Client";
import Pagination from "@/components/tools/pagination";

export default {
  name: "clients",
  layout: 'admin',
  components: {AdminNavbar, Client, Pagination}
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

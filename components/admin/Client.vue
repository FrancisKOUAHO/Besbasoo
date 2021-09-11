<template>
    <router-link :to="{name: 'admin-clientProfil'}" 
    class="banner flex flex-col w-full justify-center items-center p-8 rounded-mg bg-white rounded-lg border">
        <img class="border-4 border-white rounded-full" src="https://oasys.ch/wp-content/uploads/2019/03/photo-avatar-profil.png"/>
        <h3 class="text-lg text-center font-bold text-black-600 w-full mt-4">ESHAL Rosas</h3>
        <h3 class="text-lg text-center text-gray-500 text-left w-full">ID de l'utilisateur : #345</h3>
        <h3 class="text-lg text-center text-gray-500 text-left w-full">ESHAL.Rosas@gmail.com</h3>
        <button class="rounded-lg border font-bold text-black-600 px-8 py-1 mt-4 mr-1">
            <i class="fas fa-pen"></i>
            Profil
        </button>
    </router-link>
</template>

<style scoped>
img {
    width: 6vw;
    height: auto;
}

.banner {
    background-image: url(@/assets/images/banniere.jpg);
    background-position: center -45%;
    background-repeat: no-repeat;
    background-size: contain;
}
</style>
<template>
    <div class="flex flex-col justify-center items-center p-4 rounded-mg bg-white rounded-lg border">
        <img src="@/assets/images/image-14.png">
        <h3 class="text-lg text-left text-gray-500 w-full mt-5">Nom du produit</h3>
        <h3 class="text-lg font-bold text-black-600 text-left w-full">90.00$</h3>
        <div class="flex flex-row justify-center mt-3">
            <button class="rounded-lg border font-bold text-black-600 px-3 py-1 mr-1">
                <i class="fas fa-pen"></i>
                Modifier
            </button>
            <button class="rounded-lg border font-bold px-3 py-1 ml-1 text-red-500 hover:bg-red-500 hover:text-white">
                <i class="fas fa-trash-alt"></i>
                Supprimer
            </button>
        </div>
    </div>
</template>

<style scoped>
img {
    width: 200px;
    height: auto;
}
</style>
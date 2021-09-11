<template>

    <table class="border rounded-lg w-4/6 table-auto">
        <thead>
            <tr class="text-gray-600 uppercase text-sm leading-normal">
                <th class="py-3 px-6 text-left">Produit</th>
                <th class="py-3 px-6 text-left">Quantité</th>
                <th class="py-3 px-6 text-left">Prix</th>
                <th class="py-3 px-6 text-right">Total</th>
            </tr>
        </thead>
        <tbody class="text-sm font-light">
            <tr class="border-b border-gray-200 hover:bg-gray-100">
                <td class="py-3 px-6 text-left">
                    <div class="flex items-center">
                        <div class="mr-3">
                            <img class="w-16 h-16" src="@/assets/images/image-14.png/">
                        </div>
                        <span class="text-md text-gray-500">Tableau femme africaine</span>
                    </div>
                </td>
                <td class="py-3 px-6 text-left whitespace-nowrap">
                    <span class="text-md text-gray-500">2</span>
                </td>
                <td class="py-3 px-6 text-left whitespace-nowrap">
                    <span class="text-md text-gray-500">120.99€</span>
                </td>
                <td class="py-3 px-6 text-right whitespace-nowrap">
                    <span class="text-md text-gray-500">241.98€</span>
                </td>
            </tr>

            <!-- DUPLICATION A ENLEVER -->
            <tr class="border-b border-gray-200 hover:bg-gray-100">
                <td class="py-3 px-6 text-left">
                    <div class="flex items-center">
                        <div class="mr-3">
                            <img class="w-16 h-16" src="@/assets/images/image 5.png/">
                        </div>
                        <span class="text-md text-gray-500">Kalimba 17 lames - Golden Acacia</span>
                    </div>
                </td>
                <td class="py-3 px-6 text-left whitespace-nowrap">
                    <span class="text-md text-gray-500">2</span>
                </td>
                <td class="py-3 px-6 text-left whitespace-nowrap">
                    <span class="text-md text-gray-500">120.99€</span>
                </td>
                <td class="py-3 px-6 text-right whitespace-nowrap">
                    <span class="text-md text-gray-500">241.98€</span>
                </td>
            </tr>

            <tr class="border-b border-gray-200 hover:bg-gray-100">
                <td>
                </td>
                <td>
                </td>
                <td>
                </td>
                <td class="flex flex-col py-3 px-6 text-right whitespace-nowrap">
                    <span class="text-md">Sous-total : <span class="text-lg font-bold text-black-600">483,96€</span></span>
                    <span class="text-md">Livraison : <span class="text-lg font-bold text-black-600">Gratuite</span></span>
                    <span class="text-md">Total (TTC) : <span class="text-lg font-bold text-black-600">483,96€</span></span>
                </td>
            </tr>
            
        </tbody>
    </table>

</template>
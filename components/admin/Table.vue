<template>
    <div class="overflow-x-auto">
        <div class="min-w-screen bg-gray-100 flex items-center justify-center bg-gray-100 font-sans overflow-hidden">
            <div class="w-full lg:w-5/6">
                <div class="bg-white shadow-lg rounded-lg my-6">
                    <table class="min-w-max w-full table-auto">
                        <thead>
                            <tr class="text-gray-600 uppercase text-sm leading-normal">
                                <th class="py-3 px-6 text-left">N°Commande</th>
                                <th class="py-3 px-6 text-left">Client</th>
                                <th class="py-3 px-6 text-left">Adresse de messager</th>
                                <th class="py-3 px-6 text-center">Prix de la commande</th>
                                <th class="py-3 px-6 text-center">Statut</th>
                                <th class="py-3 px-6 text-center">Actions</th>
                            </tr>
                        </thead>
                        <tbody class="text-gray-600 text-sm font-light">
                            <tr class="border-b border-gray-200 hover:bg-gray-100">
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-bold">N°598764</span>
                                </td>
                                <td class="py-3 px-6 text-left">
                                    <div class="flex items-center">
                                        <div class="mr-3">
                                            <img class="w-8 h-8 rounded-full" src="https://media-exp1.licdn.com/dms/image/C4E03AQHwkmslAc-x5g/profile-displayphoto-shrink_200_200/0/1592513163714?e=1635379200&v=beta&t=8N9kNFJFv6E56IW5mjcI2miyijYbTcMRmNumAMPzPVA"/>
                                        </div>
                                        <span class="text-grey-900 font-light">TRUONG Jacky</span>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-light">jacky-t@hotmail.fr</span>
                                </td>
                                <td class="py-3 px-6 text-center whitespace-nowrap">
                                    <span class="font-light">778.35€</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-green-200 text-green-600 py-1 px-3 rounded-full text-xs">Délivré</span>
                                </td>
                                <td class="py-3 px-6 text-center flex justify-center">
                                    <img class="w-8 h-8 rounded-full" src="@/assets/images/icon-etc.png">
                                </td>
                            </tr>

                            <!-- DUPLICATION A ENLEVER -->
                            <tr class="border-b border-gray-200 hover:bg-gray-100">
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-bold">N°598763</span>
                                </td>
                                <td class="py-3 px-6 text-left">
                                    <div class="flex items-center">
                                        <div class="mr-3">
                                            <img class="w-8 h-8 rounded-full" src="https://media-exp1.licdn.com/dms/image/C4D03AQFG8nN7mqs5UA/profile-displayphoto-shrink_200_200/0/1627047024058?e=1635379200&v=beta&t=Bm26bQ-4SHkm_TK3C3JtHKgykeCQAElOBekZ7MBbMNs"/>
                                        </div>
                                        <span class="text-grey-900 font-light">KOUAHO Francis</span>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-light">kouahofrancis@gmail.com</span>
                                </td>
                                <td class="py-3 px-6 text-center whitespace-nowrap">
                                    <span class="font-light">199.99€</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-green-200 text-green-600 py-1 px-3 rounded-full text-xs">Délivré</span>
                                </td>
                                <td class="py-3 px-6 text-center flex justify-center">
                                    <img class="w-8 h-8 rounded-full" src="@/assets/images/icon-etc.png">
                                </td>
                            </tr>
                            <tr class="border-b border-gray-200 hover:bg-gray-100">
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-bold">N°598762</span>
                                </td>
                                <td class="py-3 px-6 text-left">
                                    <div class="flex items-center">
                                        <div class="mr-3">
                                            <img class="w-8 h-8 rounded-full" src="https://randomuser.me/api/portraits/men/1.jpg"/>
                                        </div>
                                        <span class="text-grey-900 font-light">DOE John</span>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-light">john.doe@gmail.com</span>
                                </td>
                                <td class="py-3 px-6 text-center whitespace-nowrap">
                                    <span class="font-light">9.99€</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-yellow-200 text-yellow-600 py-1 px-3 rounded-full text-xs">En transit</span>
                                </td>
                                <td class="py-3 px-6 text-center flex justify-center">
                                    <img class="w-8 h-8 rounded-full" src="@/assets/images/icon-etc.png">
                                </td>
                            </tr>
                            <tr class="border-b border-gray-200 hover:bg-gray-100">
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-bold">N°598761</span>
                                </td>
                                <td class="py-3 px-6 text-left">
                                    <div class="flex items-center">
                                        <div class="mr-3">
                                            <img class="w-8 h-8 rounded-full" src="https://oasys.ch/wp-content/uploads/2019/03/photo-avatar-profil.png"/>
                                        </div>
                                        <span class="text-grey-900 font-light">ESHAL Rosas</span>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-light">adresse@email.fr</span>
                                </td>
                                <td class="py-3 px-6 text-center whitespace-nowrap">
                                    <span class="font-light">778.35€</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-blue-200 text-blue-600 py-1 px-3 rounded-full text-xs">En traitement</span>
                                </td>
                                <td class="py-3 px-6 text-center flex justify-center">
                                    <img class="w-8 h-8 rounded-full" src="@/assets/images/icon-etc.png">
                                </td>
                            </tr>
                            <tr class="border-b border-gray-200 hover:bg-gray-100">
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-bold">N°598760</span>
                                </td>
                                <td class="py-3 px-6 text-left">
                                    <div class="flex items-center">
                                        <div class="mr-3">
                                            <img class="w-8 h-8 rounded-full" src="https://media-exp1.licdn.com/dms/image/C4E03AQHwkmslAc-x5g/profile-displayphoto-shrink_200_200/0/1592513163714?e=1635379200&v=beta&t=8N9kNFJFv6E56IW5mjcI2miyijYbTcMRmNumAMPzPVA"/>
                                        </div>
                                        <span class="text-grey-900 font-light">TRUONG Jacky</span>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-light">jacky-t@hotmail.fr</span>
                                </td>
                                <td class="py-3 px-6 text-center whitespace-nowrap">
                                    <span class="font-light">655.35€</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-red-200 text-red-600 py-1 px-3 rounded-full text-xs">Annulé</span>
                                </td>
                                <td class="py-3 px-6 text-center flex justify-center">
                                    <img class="w-8 h-8 rounded-full" src="@/assets/images/icon-etc.png">
                                </td>
                            </tr>
                            <tr class="border-b border-gray-200 hover:bg-gray-100">
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-bold">N°598759</span>
                                </td>
                                <td class="py-3 px-6 text-left">
                                    <div class="flex items-center">
                                        <div class="mr-3">
                                            <img class="w-8 h-8 rounded-full" src="https://media-exp1.licdn.com/dms/image/C4D03AQFG8nN7mqs5UA/profile-displayphoto-shrink_200_200/0/1627047024058?e=1635379200&v=beta&t=Bm26bQ-4SHkm_TK3C3JtHKgykeCQAElOBekZ7MBbMNs"/>
                                        </div>
                                        <span class="text-grey-900 font-light">KOUAHO Francis</span>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-light">kouahofrancis@gmail.com</span>
                                </td>
                                <td class="py-3 px-6 text-center whitespace-nowrap">
                                    <span class="font-light">55.79€</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-yellow-200 text-yellow-600 py-1 px-3 rounded-full text-xs">En transit</span>
                                </td>
                                <td class="py-3 px-6 text-center flex justify-center">
                                    <img class="w-8 h-8 rounded-full" src="@/assets/images/icon-etc.png">
                                </td>
                            </tr>
                            <tr class="border-b border-gray-200 hover:bg-gray-100">
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-bold">N°598758</span>
                                </td>
                                <td class="py-3 px-6 text-left">
                                    <div class="flex items-center">
                                        <div class="mr-3">
                                            <img class="w-8 h-8 rounded-full" src="https://randomuser.me/api/portraits/men/1.jpg"/>
                                        </div>
                                        <span class="text-grey-900 font-light">DOE John</span>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-light">john.doe@gmail.com</span>
                                </td>
                                <td class="py-3 px-6 text-center whitespace-nowrap">
                                    <span class="font-light">2.99€</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-red-200 text-red-600 py-1 px-3 rounded-full text-xs">Annulé</span>
                                </td>
                                <td class="py-3 px-6 text-center flex justify-center">
                                    <img class="w-8 h-8 rounded-full" src="@/assets/images/icon-etc.png">
                                </td>
                            </tr>
                            <tr class="border-b border-gray-200 hover:bg-gray-100">
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-bold">N°598757</span>
                                </td>
                                <td class="py-3 px-6 text-left">
                                    <div class="flex items-center">
                                        <div class="mr-3">
                                            <img class="w-8 h-8 rounded-full" src="https://oasys.ch/wp-content/uploads/2019/03/photo-avatar-profil.png"/>
                                        </div>
                                        <span class="text-grey-900 font-light">ESHAL Rosas</span>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <span class="font-light">adresse@email.fr</span>
                                </td>
                                <td class="py-3 px-6 text-center whitespace-nowrap">
                                    <span class="font-light">778.35€</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-blue-200 text-blue-600 py-1 px-3 rounded-full text-xs">En traitement</span>
                                </td>
                                <td class="py-3 px-6 text-center flex justify-center">
                                    <img class="w-8 h-8 rounded-full" src="@/assets/images/icon-etc.png">
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
</template>
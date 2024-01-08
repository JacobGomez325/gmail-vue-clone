<template>
  <Menu as="div" class="relative ml-3">
   <div >
     <MenuButton class="flex rounded-full  bg-primary text-sm focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800">
       <span class="sr-only">Ouvrir le menu</span>
       <img v-if="false" class="h-8 w-8 rounded-full" src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="" />
        <p class="h-8 w-8 rounded-full flex justify-center items-center bg-blue-600 text-white  text-sm uppercase f font-semibold"> 
          <span>{{ sigle }}</span>
        </p>
      </MenuButton>
   </div>
   <transition enter-active-class="transition ease-out duration-100" enter-from-class="transform opacity-0 scale-95" enter-to-class="transform opacity-100 scale-100" leave-active-class="transition ease-in duration-75" leave-from-class="transform opacity-100 scale-100" leave-to-class="transform opacity-0 scale-95">
     <MenuItems class="absolute right-0 z-10 mt-2 w-48 origin-top-right rounded-md bg-white py-1 shadow-lg ring-1 ring-black ring-opacity-5 focus:outline-none">
       <MenuItem v-slot="{ active }">
         <router-link to="#" :class="[active ? 'bg-gray-100' : '', 'block px-4 py-2 text-sm text-gray-700 font-bold']">{{userConnect.firstname}} {{ userConnect.lastname }} </router-link>
       </MenuItem>
       <hr>
       <MenuItem v-slot="{ active }">
         <router-link to="#" :class="[active ? 'bg-gray-100' : '', 'block px-4 py-2 text-sm text-gray-700']">Profil</router-link>
       </MenuItem>
       <MenuItem v-slot="{ active }">
         <router-link to="#" :class="[active ? 'bg-gray-100' : '', 'block px-4 py-2 text-sm text-gray-700']">Parametre</router-link>
       </MenuItem>
       <MenuItem v-slot="{ active }">
         <span  class=" cursor-pointer" :class="[active ? 'bg-gray-100' : '', 'block px-4 py-2 text-sm text-gray-700']">Se déconnecter</span>
       </MenuItem>
     </MenuItems>
   </transition>
 </Menu>
</template>

<script setup lang="ts">
import {reactive} from 'vue'
import { Menu, MenuButton, MenuItem, MenuItems } from '@headlessui/vue'

type User  = {
  firstname:string,
  lastname:string,
}
const userConnect = reactive({
  firstname: 'John', lastname: 'Doe'
})

const sigle = `${userConnect.firstname[0]} ${userConnect.lastname[0]}`


</script>

<style scoped>

</style>
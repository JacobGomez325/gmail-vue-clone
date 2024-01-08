<template>
  <main class="bg-gray-50">
   <TheNavbar />
   <div class="flex space-x-4">
    <TheSidebar />
    <main class="p-4 bg-white rounded-xl shadow-md border h-[80vh] overflow-auto  w-full">
      <div class="nav-content"></div>
      <div class="body-content">
       <p class="my-3" v-for="i in 30" :key="i">
        {{ i }}
       </p>
      </div>
    </main>
    <aside class="p-2 flex-col flex space-y-4">
      <span class=" block bg-gray-500 w-5 h-5"></span>
      <span class=" block bg-gray-500 w-5 h-5"></span>
      <span class=" block bg-gray-500 w-5 h-5"></span>
      <span class=" block bg-gray-500 w-5 h-5"></span>
      <span class=" block bg-gray-500 w-5 h-5"></span>
      <span class=" block bg-gray-500 w-5 h-5"></span>
    </aside>
   </div>
  </main>
</template>
<script setup lang="ts">
  import TheNavbar from '@/components/TheNavbar.vue'
  import TheSidebar from '@/components/TheSidebar.vue'

</script>



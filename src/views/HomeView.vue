<template>
  <main class="bg-gray-50">
   <TheNavbar />
   <div class="flex space-x-4">
    <TheSidebar />
    <main class="p-4 bg-white rounded-xl  shadow-md border h-screen w-full">
      En cours ....
    </main>
   </div>
  </main>
</template>
<script setup lang="ts">
  import TheNavbar from '@/components/TheNavbar.vue';
  import TheSidebar from '@/components/TheSidebar.vue';
</script>



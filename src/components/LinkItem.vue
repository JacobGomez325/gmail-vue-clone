<template>
  <router-link   class="flex items-center font-semibold py-2 px-5 z-10  relative text-gray-700 hover:bg-gray-200 hover:rounded-r-3xl transition ease-in-out duration-500  cursor-pointer  text-sm space-x-3"  :to="link">
    <span  :title="`${props.title}`" class=" ">
      <slot></slot>
    </span>
    <span >{{title}}</span>
  </router-link>
</template>

<script setup lang="ts">
  import { RouterLink} from 'vue-router'
  const props = defineProps({
    title: {
      title: String ,
      required: true
    },
    link: {
      type: String,
      default: '#'
    },
  })
  
</script>

<style  scoped>
.router-link-exact-active{
  font-weight: bold;
  background-color:#d3e3fd;
  border-right: 1px solid #d3e3fd;
  border-top-right-radius: 1.5rem/* 24px */;
  border-bottom-right-radius: 1.5rem/* 24px */;
  color: #1e293b;
  margin: 4px 0;
  
}
</style>
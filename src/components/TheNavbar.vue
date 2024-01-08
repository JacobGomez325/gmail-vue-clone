<template>
  <nav class="flex items-center p-4 justify-between">
    <div class="flex space-x-3 items-center ">
      <span><IconBarre  width="1.6em" height="1.6em" /> </span>
      <img src="/images/logo.png" class="w-[40px] h-[36px]" alt="">
      <span class="text-xl text-gray-700 font-medium">Gmail</span>
    </div>
    <InputSearch v-model="search" width="w-[60vw]" />
    <div class="flex space-x-4 items-center text-gray-600">
      <span class="cursor-pointer hover:bg-gray-100 p-1 rounded-full transition-all duration-200 "><IconQuestionMark  width="1.8em" height="2.0em" /> </span>
      <span class="cursor-pointer hover:bg-gray-100 p-1 rounded-full transition-all duration-200"><IconCog  width="1.8em" height="2.0em" /> </span>
      <span class="cursor-pointer hover:bg-gray-100 p-1 rounded-full transition-all duration-200"><IconRound  width="1.8em" height="2.0em" /> </span>
      <UserMenu />
    </div>
  </nav>
</template>

<script setup lang="ts">
import {ref} from "vue"
import IconBarre from './icons/IconBarre.vue'
import InputSearch from '@/components/InputSearch.vue'
import UserMenu from '@/components/UserMenu.vue'
import IconQuestionMark from "./icons/IconQuestionMark.vue";
import IconCog from "./icons/IconCog.vue";
import IconRound from "./icons/IconRound.vue";


const search = ref('')
</script>

<style scoped>

</style>
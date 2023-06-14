<template>
  <div class="relative  ">
    <span class="absolute text-gray-700 top-3 left-3 "><svg stroke="currentColor" fill="currentColor" stroke-width="0" version="1.1" viewBox="0 0 16 16" height="1.3em" width="1.3em" xmlns="http://www.w3.org/2000/svg"><path d="M15.504 13.616l-3.79-3.223c-0.392-0.353-0.811-0.514-1.149-0.499 0.895-1.048 1.435-2.407 1.435-3.893 0-3.314-2.686-6-6-6s-6 2.686-6 6 2.686 6 6 6c1.486 0 2.845-0.54 3.893-1.435-0.016 0.338 0.146 0.757 0.499 1.149l3.223 3.79c0.552 0.613 1.453 0.665 2.003 0.115s0.498-1.452-0.115-2.003zM6 10c-2.209 0-4-1.791-4-4s1.791-4 4-4 4 1.791 4 4-1.791 4-4 4z"></path></svg></span>
    <input type="text" v-model="value"  placeholder="Rechercher dans les messages ..." :class="props.width" class="border  border-gray-100 text-sm bg-blue-50 shadow pl-12 pr-2 py-3 outline-none rounded-3xl ">
    <span class="absolute text-gray-900 top-2 right-3 ">
      <IconAdjustement width="2.0em" height="2.0em"  />
    </span>
  </div>
</template>

<script setup lang="ts">
import { computed } from 'vue';
import type { PropType } from 'vue';
import IconAdjustement from './icons/IconAdjustement.vue';
const emits = defineEmits(['update:modelValue'])
const props = defineProps({
  modelValue:{
    required:true,
    type:String as PropType<string>
  },
  width:{
    type:String as PropType<string>,
    default:'w-full'
  }
})
const value = computed({
  get() {
    return props.modelValue
  },
  set(value) {
    emits('update:modelValue', value)
  }
})
</script>

<style>

</style>
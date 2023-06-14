<template>
  <svg xmlns="http://www.w3.org/2000/svg" :class="props.color" :height="props.height" :width="props.width" viewBox="0 0 24 24"><path fill="none" stroke="currentColor" strokeLinecap="round" strokeLinejoin="round" strokeWidth="1.5" d="M6 12L3.269 3.126A59.768 59.768 0 0 1 21.485 12A59.77 59.77 0 0 1 3.27 20.876L5.999 12Zm0 0h7.5"></path></svg>
</template>

<script setup lang="ts">
const props = defineProps({
  width: {
    type: String ,
      default: '1em'
    },
    height: {
      type: String,
      default: '1em'
    },
    color:{
      type: String ,
      default: 'currentColor'
    }
  })
</script>
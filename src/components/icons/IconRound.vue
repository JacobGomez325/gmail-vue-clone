<template>
  <svg xmlns="http://www.w3.org/2000/svg" :class="props.color" :height="props.height" :width="props.width" viewBox="0 0 24 24"><path fill="currentColor" d="M4 8h4V4H4v4zm6 12h4v-4h-4v4zm-6 0h4v-4H4v4zm0-6h4v-4H4v4zm6 0h4v-4h-4v4zm6-10v4h4V4h-4zm-6 4h4V4h-4v4zm6 6h4v-4h-4v4zm0 6h4v-4h-4v4z"></path></svg>
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
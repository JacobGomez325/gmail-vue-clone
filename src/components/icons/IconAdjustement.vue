<template>
  <svg xmlns="http://www.w3.org/2000/svg" :class="props.color" :height="props.height" :width="props.width" viewBox="0 0 24 24"><path fill="currentColor" d="M18.75 12.75h1.5a.75.75 0 0 0 0-1.5h-1.5a.75.75 0 0 0 0 1.5ZM12 6a.75.75 0 0 1 .75-.75h7.5a.75.75 0 0 1 0 1.5h-7.5A.75.75 0 0 1 12 6Zm0 12a.75.75 0 0 1 .75-.75h7.5a.75.75 0 0 1 0 1.5h-7.5A.75.75 0 0 1 12 18ZM3.75 6.75h1.5a.75.75 0 1 0 0-1.5h-1.5a.75.75 0 0 0 0 1.5Zm1.5 12h-1.5a.75.75 0 0 1 0-1.5h1.5a.75.75 0 0 1 0 1.5ZM3 12a.75.75 0 0 1 .75-.75h7.5a.75.75 0 0 1 0 1.5h-7.5A.75.75 0 0 1 3 12Zm6-8.25a2.25 2.25 0 1 0 0 4.5a2.25 2.25 0 0 0 0-4.5ZM12.75 12a2.25 2.25 0 1 1 4.5 0a2.25 2.25 0 0 1-4.5 0ZM9 15.75a2.25 2.25 0 1 0 0 4.5a2.25 2.25 0 0 0 0-4.5Z"></path></svg>
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
<template>
  <div class="w-[25%]">
    <div class="flex justify-center">
      <button class="flex space-x-3 items-center bg-[#c2e7ff] rounded-xl p-4">
        <span class="text-gray-700"><IconPencil width="1.5em" height="1.5em" /></span>
        <span class="text-sm font-medium">Nouveau message</span>
      </button>
    </div>
    <div class="pt-3 pb-6">
      <ul>
        <link-item link="/" title="Boites de recep..."> <IconInbox  width="1.5em" height="1.5em" /> </link-item>
        <link-item link="/message" title="Messages Suivis"> <IconStar width="1.5em" height="1.5em" /> </link-item>
        <link-item link="/attente" title="En attente"> <IconClock width="1.5em" height="1.5em" /> </link-item>
        <link-item link="/send" title="Message envoyés"> <IconAirplaine width="1.5em" height="1.5em" /> </link-item>
        <link-item link="/brouillon" title="Brouillons"> <IconDocument width="1.5em" height="1.5em" /> </link-item>
        <link-item link="/plus" title="Plus"> <IconChevronDown width="1.5em" height="1.5em" /> </link-item>
        
      </ul>
    </div>
  </div>
</template>

<script setup lang="ts">
  import LinkItem from './LinkItem.vue'
  import IconInbox from '@/components/icons/IconInbox.vue'
  import IconStar from '@/components/icons/IconStar.vue'
  import IconClock from '@/components/icons/IconClock.vue'
  import IconAirplaine from '@/components/icons/IconAirplaine.vue'
  import IconDocument from '@/components/icons/IconDocument.vue'
  import IconPencil from '@/components/icons/IconPencil.vue'
  import IconChevronDown from '@/components/icons/IconChevronDown.vue'
  import IconPlus from '@/components/icons/IconPlus.vue'
</script>

<style scoped>

</style>
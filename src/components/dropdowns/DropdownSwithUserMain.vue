<script setup>
const props = defineProps({ label: String });
</script>

<template>
  <div class="m-2 flex">
    <div class="m-2">
      <img
        :src="`https://picsum.photos/seed/${label}/560/315`"
        alt="video_preview"
        class="h-12 w-12 rounded-full border-2 border-blue-400"
      />
    </div>
    <div class="flex flex-col items-start">
      <span class="text-sm">John Doe</span>
      <span class="text-xs text-[#aaaaaa]">example@mail.com</span>
      <span class="text-xs text-[#aaaaaa]">No subscribrs</span>
    </div>
  </div>
  <div class="border-b border-[#555555] p-4 text-start text-sm">
    View all channel
  </div>
  <div class="flex items-center gap-2 p-2 hover:bg-[#555555]">
    <BaseIcon name="add-account" class="h-8" /><span>Add account</span>
  </div>
  <div class="flex items-center gap-2 p-2 hover:bg-[#555555]">
    <BaseIcon name="user-signout" class="h-8" />
    <span>Sign out</span>
  </div>
</template>

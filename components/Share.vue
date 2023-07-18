<template>
  <div class="cursor-pointer">
    <div class="flex justify-center" @click="open = true">
      <p class="text-blue-600 font-bold text-lg">Share</p>
    </div>

    <ShareModal v-model="open" />
  </div>
</template>

<script setup>
let open = ref(false);
</script>

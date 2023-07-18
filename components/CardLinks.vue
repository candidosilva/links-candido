<template>
  <div
    class="bg-white flex items-center w-full mx-4 max-w-md p-4 rounded-full shadow-lg shadow-red-500 cursor-pointer"
    @click="irPara(link.link)"
  >
    <Icon :name="`mdi:${link.icone}`" class="-mr-8" size="32" color="tomato" />

    <p class="font-bold px-2 m-auto text-center">{{ link.texto }}</p>
  </div>
</template>

<script setup>
defineProps({
  link: {
    type: Object,
  },
});

function irPara(link) {
  window.open(link, "_blank");
}
</script>

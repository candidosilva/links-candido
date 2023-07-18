<template>
  <div class="w-screen h-screen bg-gradient-to-br from-red-400 to-sky-200">
    <div class="flex justify-center items-center pt-4">
      <Avatar />
    </div>

    <div class="text-center text-white text-xl font-medium mt-2 pb-4">
      <h1>Coding Station</h1>
      <h1>Cândido Silva</h1>
    </div>

    <div class="flex flex-col items-center px-4">
      <CardLinks
        v-for="(link, idx) in links"
        :key="idx"
        :link="link"
        class="mt-6"
      />
    </div>

    <Share class="mt-8" />
  </div>
</template>

<script setup>
useHead({
  title: "Coding Station",
});

const links = [
  {
    link: "https://www.youtube.com/channel/UCRf0nh12CLg_S9khtuEMfQQ",
    texto: "Youtube",
    icone: "youtube",
  },
  {
    link: "https://www.instagram.com/codingstation_/",
    texto: "Instagram",
    icone: "instagram",
  },
  {
    link: "https://www.linkedin.com/in/candido-silva-developer/",
    texto: "Linkedin",
    icone: "linkedin",
  },
];
</script>

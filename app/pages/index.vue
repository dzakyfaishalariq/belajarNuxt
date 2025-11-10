<script setup lang="ts">
const fetur = ref([
  {
    title: "Happy",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur eaque repellendus eveniet error autem, assumenda doloribus repellat ratione voluptas debitis cum neque veniam, commodi placeat consectetur ullam excepturi id nisi.",
    icon: "i-lucide-smile",
    to: "/",
  },
  {
    title: "Semangat",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur eaque repellendus eveniet error autem, assumenda doloribus repellat ratione voluptas debitis cum neque veniam, commodi placeat consectetur ullam excepturi id nisi.",
    icon: "i-lucide-a-large-small",
    to: "/",
  },
  {
    title: "Taqwa",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur eaque repellendus eveniet error autem, assumenda doloribus repellat ratione voluptas debitis cum neque veniam, commodi placeat consectetur ullam excepturi id nisi.",
    icon: "i-lucide-sun-moon",
    to: "/",
  },
]);
</script>
<template>
  <div>
    <UPageSection
      title="Home"
      description="Aplikasi ini hanya untuk perkenalan saja dan merupakan aplikasi untuk uji coba"
      icon="i-lucide-rocket"
      :features="fetur"
    />
  </div>
</template>

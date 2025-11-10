<script setup lang="ts">
import type { NavigationMenuItem } from "@nuxt/ui";
// inisialisais route
const route = useRoute();
// inisialisasi items menu navbar
const items = computed<NavigationMenuItem[]>(() => [
  {
    label: "Home",
    to: "/",
  },
  {
    label: "About",
    to: "/about",
    active: route.path.startsWith("/about"),
  },
  {
    labol: "Content",
    to: "/content",
    active: route.path.startsWith("/content"),
  },
]);

const itemsFooter = computed<NavigationMenuItem[]>(() => [
  {
    label: "My Github",
    to: "https://github.com/dzakyfaishalariq",
    target: "_blank",
  },
]);
</script>
<template>
  <div>
    <UApp>
      <!-- header -->
      <UHeader>
        <template #title>
          <h1 class="text-2xl font-bold">Aplikasi</h1>
        </template>
        <UNavigationMenu :items="items" />
      </UHeader>
      <UMain>
        <slot />
      </UMain>
      <!-- footer -->
      <UFooter>
        <template #left>
          <p class="text-muted text-sm">
            Copyright © 2025 by Dzaky Faishalariq
          </p>
        </template>
        <UNavigationMenu :items="itemsFooter" variant="link" />
      </UFooter>
    </UApp>
  </div>
</template>

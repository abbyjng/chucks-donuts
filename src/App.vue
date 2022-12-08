<script setup>
import { ref } from "vue";

import TheHeader from "./components/TheHeader.vue";
import HomePage from "./components/HomePage.vue";
import AboutPage from "./components/AboutPage.vue";
import MenuPage from "./components/MenuPage.vue";

const page = ref("home"); // what page is visible

// changes page (basically acts as a link)
function pageChanged(in_page) {
  page.value = in_page;
}
</script>

<template>
  <header>
    <TheHeader @pageChanged="pageChanged" />
  </header>

  <main>
    <HomePage v-if="page == 'home'" @pageChanged="pageChanged" />
    <AboutPage v-if="page == 'about'" @pageChanged="pageChanged" />
    <MenuPage v-if="page == 'menu'" @pageChanged="pageChanged" />
  </main>
</template>

<style scoped></style>

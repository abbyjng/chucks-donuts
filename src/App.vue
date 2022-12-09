<script setup>
import { ref } from "vue";

import TheHeader from "./components/TheHeader.vue";
import HomePage from "./components/HomePage.vue";
import AboutPage from "./components/AboutPage.vue";
import MenuPage from "./components/MenuPage.vue";
import TheFooter from "./components/TheFooter.vue";

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
    <TheFooter />
  </main>
</template>

<style scoped>
main {
  flex-grow: 1;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
</style>

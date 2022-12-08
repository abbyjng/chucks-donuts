<script setup>
import { ref } from "vue";

const glazedOpen = ref(false);
const fritterOpen = ref(false);
const sandwichOpen = ref(false);

function readMore(listing) {
  if (listing == "glazed") {
    glazedOpen.value = !glazedOpen.value;
  } else if (listing == "fritter") {
    fritterOpen.value = !fritterOpen.value;
  } else if (listing == "sandwich") {
    sandwichOpen.value = !sandwichOpen.value;
  }
}
</script>

<template>
  <h1>Menu</h1>
  <div id="menu-grid">
    <div class="menu-item">
      <img src="./images/glazed.png" />
      <hr />
      <h2>Classic Glazed*</h2>
      <span>$1.00</span>
      <br />
      <a href="#" @click="readMore('glazed')">{{
        glazedOpen ? "Hide" : "Read more"
      }}</a>
      <div v-if="glazedOpen">glazed!</div>
    </div>
    <div class="menu-item">
      <img src="./images/chocolate_glazed.png" />
      <hr />
      <h2>Chocolate Glazed</h2>
      <span>$1.00</span>
    </div>
    <div class="menu-item">
      <img src="./images/sprinkle.png" />
      <hr />
      <h2>Sprinkled</h2>
      <span>$1.00</span>
    </div>
    <div class="menu-item">
      <img src="./images/chocolate_cake.png" />
      <hr />
      <h2>Chocolate Cake</h2>
      <span>$1.00</span>
    </div>
    <div class="menu-item">
      <img src="./images/apple_fritter.png" />
      <hr />
      <h2>Apple Fritter*</h2>
      <span>$1.50</span>
      <br />
      <a href="#" @click="readMore('fritter')">{{
        fritterOpen ? "Hide" : "Read more"
      }}</a>
      <div v-if="fritterOpen">fritter!</div>
    </div>
    <div class="menu-item">
      <img src="./images/egg_sandwich.png" />
      <hr />
      <h2>Egg Sandwich*</h2>
      <span>$4.50</span>
      <br />
      <a href="#" @click="readMore('sandwich')">{{
        sandwichOpen ? "Hide" : "Read more"
      }}</a>
      <div v-if="sandwichOpen">sandwich!</div>
    </div>
  </div>
</template>

<style scoped>
#menu-grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  row-gap: 30px;
}

.menu-item {
  text-align: center;
  padding: 10px;
}

img {
  width: 100%;
}

h1 {
  text-align: center;
}

h2 {
  margin-top: 20px;
}
</style>

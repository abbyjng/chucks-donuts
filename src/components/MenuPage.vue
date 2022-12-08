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
      <div v-if="glazedOpen">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc non risus
        placerat, posuere est non, iaculis mi. Nullam fermentum id nisi sit amet
        vulputate. Vestibulum massa nisi, dignissim eu nibh viverra, rutrum
        ullamcorper ante. Suspendisse eget sem dolor. Proin a lectus turpis.
        Integer hendrerit erat at placerat dignissim. Aenean vitae mi est.
        Aliquam erat volutpat. Nunc luctus varius velit ut pulvinar. Maecenas
        nec hendrerit diam. Pellentesque habitant morbi tristique senectus et
        netus et malesuada fames ac turpis egestas. Aliquam augue quam,
        convallis ut dui nec, molestie consequat quam. Suspendisse semper est
        massa, a condimentum lorem rutrum eget. Pellentesque laoreet enim et
        malesuada luctus. Quisque mattis risus vel fringilla lacinia.
        Suspendisse sodales turpis leo, laoreet blandit tortor laoreet eget.
        Etiam commodo maximus magna, nec viverra nibh rutrum vitae. Donec nisi
        massa, consequat ac libero ut, elementum rutrum est. Cras varius ornare
        velit, in fermentum mi cursus ullamcorper. Maecenas consectetur sed
        ligula sed molestie. Nullam in lobortis diam. Maecenas ullamcorper
        sagittis est, a commodo odio porta ac. Integer imperdiet mauris ut
        imperdiet interdum. Praesent ac egestas nibh. Sed sit amet faucibus
        ipsum. Nullam ac risus enim. Vivamus iaculis, tortor eget sodales
        viverra, ante ligula efficitur dolor, sed volutpat risus quam et mi.
      </div>
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

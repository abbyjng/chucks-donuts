<script setup></script>

<template>
  <div id="homepage">
    <img src="./images/box.png" />
    <div>
      <h1>Welcome to Chuck's Donuts!</h1>
      <span
        >Come visit us in Los Angeles to get a taste of our donuts! If you have
        questions, contact us at
      </span>
      <a href="#">chucksdonuts@gmail.com</a>
      <span> or give us a call at </span>
      <a href="#">(123) 456-7890</a>.
    </div>
  </div>
</template>

<style scoped>
img {
  width: 100%;
}

@media (min-width: 1000px) {
  img {
    width: 60%;
  }

  #homepage {
    display: flex;
    gap: 20px;
    align-items: center;
  }
}
</style>

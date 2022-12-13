<script setup></script>

<template>
  <div class="header">
    <a @click="$emit('pageChanged', 'home')" href="#">
      <img src="./images/logo.png" />
    </a>
    <div class="nav-links">
      <a @click="$emit('pageChanged', 'home')" href="#">Home</a>
      <a @click="$emit('pageChanged', 'about')" href="#">About Us</a>
      <a @click="$emit('pageChanged', 'menu')" href="#">Menu</a>
    </div>
  </div>
</template>

<style scoped>
.header {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
}

.nav-links {
  display: flex;
  font-family: Rockwell, "Arvo";
  flex-direction: column;
}

.nav-links a {
  padding: 10px;
  text-decoration: none;
}

img {
  height: 40px;
  display: none;
}

@media (min-width: 600px) {
  img {
    display: block;
  }

  .nav-links {
    flex-direction: row;
  }
}
</style>

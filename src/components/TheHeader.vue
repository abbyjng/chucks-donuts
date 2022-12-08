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
}

.nav-links a {
  padding: 10px;
  text-decoration: none;
}

img {
  height: 40px;
}
</style>

<script setup>
import { RouterLink, RouterView } from "vue-router";
import AsideView from "./views/AsideView.vue";
</script>

<template>
  <AsideView />
  <main>
    <router-view />
  </main>
</template>

<style scoped>
main {
  background: #0d0d0d;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 2rem;
  height: 100vh;
}

main > section {
  width: 100%;
  height: 100%;
  background-color: #212121;
}

.content-container {
  background-color: rgb(255, 255, 255);
}
</style>

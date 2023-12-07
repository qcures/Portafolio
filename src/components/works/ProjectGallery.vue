<script setup>
import { ref, watch } from "vue";
import { database } from "./../../database/database.js";
const props = defineProps({
  activeSection: String,
});

const show = ref(`${props.activeSection}`);

watch(show, (newX) => {
  console.log(`x is ${newX}`);
});

/* 

3. mostrar proyectos con un v-for

1. crear un slider que va a contener todas las imagenes

2. crear los botones de previous - next para moverse por el slider


*/
</script>

<template>
  <div id="gallery">
    <div class="slider"></div>
  </div>
</template>

<style lang="scss" scoped></style>

<script setup>
import { ref } from "vue";
import { database } from "./../database/database.js";

const activeSection = ref("none");
const show = ref([]);

function select(direction) {
  show.value = database;
  if (direction == "left") {
    show.value = database.filter((e) => e.category == "photos");
  }
  if (direction == "right") {
    show.value = database.filter((e) => e.category == "design");
  }
  activeSection.value = direction;
}
</script>

<template>
  <section :class="activeSection">
    <div id="gallery">
      <div class="slider">
        <div v-for="(p, i) in show" :key="`p${i}`">
          <h1>title: {{ p.title }}</h1>
          <div v-for="(img_url, j) in p.images">
            <img
              :src="`https://drive.google.com/uc?export=view&id=${img_url}`"
              :key="`img${j}`"
              alt="project image"
            />
          </div>
        </div>
      </div>
    </div>
    <div
      class="left-div"
      @click="select('left')"
      :class="activeSection == 'left' ? 'activate' : ''"
    >
      photos
    </div>
    <div
      class="right-div"
      @click="select('right')"
      :class="activeSection == 'right' ? 'activate' : ''"
    >
      design
    </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  text-transform: uppercase;
  padding: 1rem;
  transition: all 100ms;
  display: flex;
  position: relative;
}

section > div {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 50%;
  height: 100%;
  transition: all 1000ms;
  overflow: hidden;
}

.right-div {
  background-color: black;
  color: white;
}

.left-div {
  background-color: white;
  color: black;
}

.activate {
  width: 100%;
}

section.left > .right-div {
  width: 0px;
}

section.right > .left-div {
  width: 0px;
}

#gallery {
  position: absolute;
  width: calc(100% - 2rem);
  height: calc(100% - 2rem);
  background-color: aliceblue;
  opacity: 0;
  display: none;
  animation: showGallery 1000ms 1500ms forwards linear;
}

section.left > #gallery,
section.right > #gallery {
  display: flex;
}

@keyframes showGallery {
  to {
    opacity: 1;
  }
}
</style>

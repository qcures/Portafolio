<script setup></script>

<template>
  <aside>
    <div class="aside-container">
      <h1>DANIEL CURE</h1>
      <router-link to="/works" class="nav-link" active-class="active-link"
        >works</router-link
      >
      <router-link to="/shop" class="nav-link" active-class="active-link"
        >shop</router-link
      >
      <router-link to="/about" class="nav-link about" active-class="active-link"
        >about</router-link
      >
      <router-link to="/contact" class="nav-link" active-class="active-link"
        >contact</router-link
      >
    </div>
  </aside>
</template>

<style lang="scss" scoped>
aside {
  background: #000;
  height: 100vh;
  font-family: Helvetica;
  padding: 20px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.aside-container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

h1 {
  color: var(--color-heading);
  font-family: "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue",
    Helvetica, Arial, "Lucida Grande", sans-serif;
  font-size: 63.59px;
  font-weight: 700;
  line-height: normal;
  text-align: center;
  margin-bottom: 20px;
}

.nav-link,
.about {
  color: var(--color-text);
  font-family: Helvetica;
  font-size: 31.79px;
  font-weight: 300;
  line-height: normal;
  font-style: oblique;
  text-decoration: none;
  display: block;
  margin-bottom: 5px;
}

/* Style for the active link */
.active-link {
  color: white;
}
</style>

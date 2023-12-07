<script setup>
let name = "";
let email = "";
let phone = "";

const handleSubmit = () => {
  console.log("Name:", name);
  console.log("Email:", email);
  console.log("Phone:", phone);
};
</script>

<template>
  <section>
    <div class="contact-section">
      <div class="contact-form">
        <label for="name" class="form-label">NAME</label>
        <input v-model="name" type="text" id="name" class="form-input" />

        <label for="email" class="form-label">EMAIL</label>
        <input v-model="email" type="email" id="email" class="form-input" />

        <label for="phone" class="form-label">PHONE</label>
        <input v-model="phone" type="tel" id="phone" class="form-input" />

        <button @click="handleSubmit" class="submit-button">SUBMIT</button>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.ig-link {
  position: absolute;
  left: 85%;
  top: 25%;
  padding: 0;
  border: none;
  background: none;
  cursor: pointer;
}

.tw-link {
  position: absolute;
  left: 90%;
  top: 25%;
  padding: 0;
  border: none;
  background: none;
  cursor: pointer;
}

h1 {
  position: absolute;
  left: 45%;
  top: 23%;
  font-family: "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue",
    Helvetica, Arial, "Lucida Grande", sans-serif;
  font-size: 63.59px;
  font-weight: 700;
  line-height: normal;
  text-align: center;
}

h2 {
  color: rgb(61, 61, 61);
  position: absolute;
  left: 46%;
  top: 31%;
  font-family: "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue",
    Helvetica, Arial, "Lucida Grande", sans-serif;
}

.bio-text {
  position: absolute;
  left: 46%;
  top: 37%;
  font-family: "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue",
    Helvetica, Arial, "Lucida Grande", sans-serif;
  font-size: 22.11px;
}

section {
  text-transform: uppercase;
  padding: 1rem;
  display: flex;
  position: relative;
  align-items: center;
  justify-content: center;
}

.contact-section {
  background: white;
  width: 100%;
  height: 100%;
}

section > div {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 50%;
  height: 100%;
}

.image-frame {
  position: absolute;
  left: 5%;
  background: black;
  width: 407.44px;
  height: 523.85px;
}

.image-container {
  background: red;
  width: 381px;
  height: 490px;
  margin: 54px;
}

.image-container > img {
  object-fit: cover;
  width: 100%;
  height: 100%;
}

.contact-form {
  display: flex;
  flex-direction: column;
  align-items: flex-start; /* Align items to the start (left) of the container */
  padding: 1rem; /* Add padding for better spacing */
}

.form-label {
  width: 511.9px;
  height: 41.01px;
  stroke-width: 1px;
  stroke: #000;
  color: #000;
  font-family: "Helvetica Neue", sans-serif;
  font-size: 50.03px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
  margin-bottom: 0.9rem;
}

.form-input {
  width: 511.9px;
  height: 41.01px;
  stroke-width: 1px;
  stroke: #000;
  color: #000;
  font-family: "Helvetica Neue", sans-serif;
  font-size: 24px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  margin-bottom: 1rem;
  padding: 0.5rem;
}

.submit-button {
  font-family: "Helvetica Neue", sans-serif;
  font-style: normal;
  font-weight: 500;
  font-size: 25px;
  align-self: flex-end; /* Align to the right end */
  background-color: black;
  color: white;
  width: 185.05px;
  height: 41.01px;
  border: none;
  cursor: pointer;
}
</style>

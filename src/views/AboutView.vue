<script setup></script>

<template>
  <section>
    <div class="about-section">
      <div class="image-frame">
        <div class="image-container">
          <img
            src="https://media.discordapp.net/attachments/1037916469410926672/1077726507444740228/image.png?ex=6578e606&is=65667106&hm=8e390365368d74b6af5df942e428f3f8ae22665f6e5e01a7e483df5b475736b4&=&format=webp&quality=lossless&width=1132&height=858"
            alt=""
            srcset=""
          />
        </div>
      </div>
      <button class="ig-link">
        <img
          src="https://cdn.discordapp.com/attachments/1037916469410926672/1181378462691364874/IG_ICON.png?ex=6580d76e&is=656e626e&hm=04b5da5b03c1f1200ce50aceb9a469a8a2f7814d67aab411454392061ca54f94&"
          onclick="window.location.href='https://www.instagram.com/shotbycure/';"
          alt="buttonpng"
        />
      </button>
      <button class="tw-link">
        <img
          src="https://cdn.discordapp.com/attachments/1037916469410926672/1181378463098220684/TWITTER_ICON.png?ex=6580d76e&is=656e626e&hm=a3567c70082ee277e774ce3e6d1a3a8fc7b235369603da81dbeeb231c2230eae&"
          onclick="window.location.href='https://www.twitter.com/shotbycure/';"
          alt="buttonpng"
        />
      </button>
      <h1>DANIEL CURE</h1>
      <H2>Photographer/Designer</H2>
      <p class="bio-text">
        Expressing my thoughts freely in my work is my greatest passion.
      </p>
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

.about-section {
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
  width: 381px;
  height: 490px;
  margin: 54px;
}

.image-container > img {
  object-fit: cover;
  width: 100%;
  height: 100%;
}
</style>

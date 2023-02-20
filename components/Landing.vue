<template>
  <div class="invitation">
    <div class="main-data-container">
      <div class="landing-data-container">
        <div class="title-container">
          <span class="title">
            Richie's fest
          </span>
        </div>
        <div class="album-cover-container">
          <img
            class="album-cover"
            src="@/assets/la_woman_photo.webp"
          >
        </div>
        <div class="subtitle-container">
          <span class="subtitle">
            25 de febrero 2023
          </span>
        </div>
      </div>
    </div>
    <div class="scroll-down-container">
      <scroll-down-arrow href="#location" />
    </div>
  </div>
</template>

<script>
import ScrollDownArrow from '@/components/ScrollDownArrow'

export default {
  components: {
    ScrollDownArrow
  }
}
</script>

<style>
.invitation {
  height: 100%;
  width: 100%;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.scroll-down-container{
  width: 100%;
  height: 15%;
}

.main-data-container{
  width: 100%;
  height: 85%;

  padding-top: 100px;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.landing-data-container{
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.title-container{
  width: 70%;
  text-align: left;
  margin-top: 15px;
}

.album-cover-container {
  width: 70%;
  margin: auto;
}

.title{
  font-family: var(--title-font);
  color: var(--light-shades);
  font-size: 6vh;
}

.album-cover{
  width: 100%;
}

.subtitle-container{
  width: 80%;
  margin-top: 30px;
  text-align: center;
  letter-spacing: 1.5px;
}

.subtitle{
  color: var(--dark-shades);
  font-size: 2.6vh;
  font-family: var(--subtitle-font);
}

@media only screen and (min-width: 768px) {
  .subtitle-container{
    width: 50%;
  }

  .title{
    font-size: 9vh;
  }

  .title-container{
    width: 60%;
  }
}
</style>

<template>
  <div class="invitation invite-image">
    <div class="landing-data-container">
      <boombox />
      <div class="title-container">
        <span class="title pink-neon-text">
          ¡Mis 60!
        </span>
      </div>
      <div class="subtitle-container">
        <span class="subtitle">
          ven a festejar en grande mi cumpleaños este <span class="date-highlight">8 de octubre</span>
        </span>
      </div>
    </div>
    <div class="scroll-down-container">
      <scroll-down-arrow href="#location" />
    </div>
  </div>
</template>

<script>
import Boombox from '@/components/Boombox.vue'
import ScrollDownArrow from '@/components/ScrollDownArrow'

export default {
  components: {
    Boombox,
    ScrollDownArrow
  }
}
</script>

<style>
.scroll-down-container{
  width: 100%;
  height: 15%;
}

.landing-data-container{
  width: 100%;
  height: 85%;

  padding-top: 100px;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.invitation {
  height: 100%;
  width: 100%;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.title-container{
  width: 90%;
  text-align: center;
  margin-top: 15px;
}

.title{
  font-family: var(--title-font);
  font-size: 6vh;
}

.subtitle-container{
  width: 80%;
  margin-top: 60px;
  text-align: center;
  letter-spacing: 1.5px;
}

.subtitle{
  color: var(--light-shades);
  font-size: 2.6vh;
  font-family: var(--subtitle-font);
}

.date-highlight{
  color: var(--purple-main-color);
}

@media only screen and (min-width: 768px) {
  .subtitle-container{
    width: 50%;
  }

  .title{
    font-size: 10vh;
  }

  .title-container{
    width: 60%;
  }
}
</style>

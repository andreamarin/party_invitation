<template>
  <div class="holder">
    <div class="all-sections">
      <div id="landing" class="main-section">
        <!-- <landing /> -->
        <neon-landing />
      </div>
      <div id="location" class="section">
        <location />
      </div>
    </div>
    <div class="landing-menu-container">
      <Slide :close-on-navigation="true" no-overlay>
        <a id="landing-menu" href="#landing">
          <span>Inicio</span>
        </a>
        <a id="location-menu" href="#location">
          <span>Lugar</span>
        </a>
        <a id="dressCode-menu" href="#dress-code">
          <span>Vestimenta</span>
        </a>
        <a id="faq-menu" href="#faq">
          <span>Preguntas frecuentes</span>
        </a>
      </Slide>
    </div>
  </div>
</template>

<script>
// import Landing from '@/components/Landing'
import NeonLanding from '@/components/NeonLanding'
import Location from '@/components/Location'
import { Slide } from 'vue-burger-menu'

export default {
  components: {
    Location,
    // Landing,
    Slide,
    NeonLanding
  },
  head: {
    bodyAttrs: {
      class: 'main-body'
    }
  }
}
</script>

<style>
.holder{
  display: block;
  position: relative;
  height: 100%;
}

.landing-menu-container{
  position: fixed;
  top: 5px;
}

.all-sections {
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;
}

.main-section {
  height: 100vh;
  width: 100%;
}

.section {
  min-height: 100vh;
  width: 100%;
  margin-top: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}

/* burger menu config */
.bm-burger-bars {
  background-color: var(--dark-accent);
}

.bm-menu {
  background-color: var(--dark-accent);
  color: var(--light-shades);
}

.bm-cross {
  background-color: var(--light-shades);
}

.bm-burger-button{
  background-color: var(--light-accent);
  border-radius: 25px;
  width: 85px;
  height: 50px;
}

.line-style {
  height: 12%;
  width: 60%;
  margin: auto;
}

div.bm-burger-button > :first-child {
  top: 25% !important;
}

div.bm-burger-button > :nth-child(2) {
  top: 45% !important;
}

div.bm-burger-button > :last-child {
  top: 65% !important;
}
</style>

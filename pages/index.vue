<template>
  <div class="holder">
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
    <div class="all-sections">
      <div id="landing" class="main-section">
        <landing />
      </div>
      <!-- <div id="location" class="section">
        <location />
      </div> -->
    </div>
  </div>
</template>

<script>
// import Landing from '@/components/Landing'
// import Location from '@/components/Location'
import { Slide } from 'vue-burger-menu'

export default {
  components: {
    // Location,
    // Landing,
    Slide
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
  position: relative;
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
  height: 500px;
  width: 100%;
}

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
  position: relative;
}
</style>

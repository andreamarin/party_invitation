<template>
  <div>
    <Slide :close-on-navigation="true">
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
      <div id="location" class="section">
        <location />
      </div>
      <div id="dress-code" class="section">
        <dress-code />
      </div>
      <div id="faq" class="section">
        <faq />
      </div>
    </div>
  </div>
</template>

<script>
import Landing from '@/components/Landing'
import DressCode from '@/components/DressCode'
import Location from '@/components/Location'
import Faq from '@/components/Faq'
import { Slide } from 'vue-burger-menu'

export default {
  components: {
    Location,
    Landing,
    DressCode,
    Faq,
    Slide
  },
  data () {
    return {
      open: true
    }
  }
}
</script>

<style>
.all-sections {
  width: 100%;
  display: flex;
  flex-direction: column;
}
.main-section {
  height: 800px;
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
</style>

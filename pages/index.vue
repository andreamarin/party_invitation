<template>
  <div class="holder">
    <div class="all-sections">
      <div id="landing" class="main-section">
        <landing />
      </div>
      <div class="other-sections">
        <location id="location" />
        <dress-code id="dress-code" />
        <faq id="faq" />
      </div>
      <div class="main-section">
        <goodbye />
      </div>
    </div>
    <div class="menu-container">
      <Slide :close-on-navigation="true" no-overlay>
        <a id="landing-menu" v-scroll-to="'#landing'" href="#">
          <span>Inicio</span>
        </a>
        <a id="location-menu" v-scroll-to="'#location'" href="#">
          <span>Lugar</span>
        </a>
        <a id="dressCode-menu" v-scroll-to="'#dress-code'" href="#">
          <span>Vestimenta</span>
        </a>
        <a id="faq-menu" v-scroll-to="'#faq'" href="#">
          <span>Preguntas frecuentes</span>
        </a>
      </Slide>
    </div>
  </div>
</template>

<script>
import DressCode from '@/components/DressCode'
import Faq from '@/components/Faq'
import Goodbye from '@/components/Goodbye'
import Landing from '@/components/Landing'
import Location from '@/components/Location'
import { Slide } from 'vue-burger-menu'

export default {
  components: {
    DressCode,
    Faq,
    Goodbye,
    Location,
    Landing,
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
.other-sections {
  padding-bottom: 50px;
}

.holder{
  display: block;
  position: relative;
  height: 100%;
}

.menu-container{
  position: fixed;
  top: 0px;
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
  width: 100%;
}

/* burger menu config */
.bm-burger-bars {
  background-color: #8F43B6;
}

.bm-menu {
  background-color: var(--dark-shades);
  color: var(--light-shades);
}

.bm-cross {
  background-color: var(--light-shades);
}

.bm-burger-button{
  background-color: rgba(240, 231, 238, 0.7);
  border: var(--light-shades) 2px solid;
  border-radius: 25px;
  width: 60px;
  height: 35px;
}

.line-style {
  height: 12%;
  width: 60%;
  margin: auto;
  border-radius: 10px;
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

@media only screen and (min-width: 768px) {
.bm-burger-button{
  width: 85px;
  height: 50px;
}

.line-style {
  height: 12%;
}
}
</style>

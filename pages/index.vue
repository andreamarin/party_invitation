<template>
  <div class="holder">
    <div class="all-sections">
      <div id="landing" class="main-section">
        <landing />
      </div>
      <div class="other-sections">
        <ceremony id="location" />
      </div>
    </div>
  </div>
</template>

<script>
import Landing from '@/components/Landing'
import Ceremony from '@/components/Ceremony'

export default {
  components: {
    Ceremony,
    Landing
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

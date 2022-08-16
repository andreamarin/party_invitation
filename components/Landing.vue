<template>
  <div class="invitation invite-image">
    <div class="title-container">
      <!-- <boombox /> -->
      <span class="title title-neon">
        ¡Mi cumpleaños 60!
      </span>
    </div>
    <div class="subtitle-container">
      <span class="subtitle">
        Acompañame este 8 de octubre a las 13:00hrs a festejar en grande.

        Laura
      </span>
    </div>
    <!-- TODO: flecha de detalles -->
  </div>
</template>

<script>
// import Boombox from './Boombox.vue'

export default {
  // components: { Boombox }
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
  column-gap: 20px;
}
.title-container{
  margin-bottom: 0;
  width: 60%;
  text-align: center;
}
.title{
  font-family: var(--title-font);
  color: #FFADFE;
  font-size: 8rem;
}
.subtitle-container{
  width: 50%;
  text-align: center;
  margin-top: 0;
}
.subtitle{
  color: var(--dark-accent);
  font-size: 2rem;
  font-family: var(--subtitle-font);
}
.title-neon {
  text-shadow:
    0 0 3px rgba(255,194,254,0.98),
    0 0 30px rgba(255,194,254,0.34),
    0 0 12px rgba(255,10,251,0.52),
    0 0 22px rgba(255,10,251,0.92),
    0 0 38px rgba(255,10,251,0.78),
    0 0 60px rgba(255,10,251,0.92);
}
.title-flicker {
  color: #FFD9EB;
  animation: neon .08s ease-in-out infinite alternate;
}
.title-blue {
  color: #c6e2ff;
  text-shadow:
    0 0 2px rgba(202,228,225,0.92),
    0 0 10px rgba(202,228,225,0.34),
    0 0 4px rgba(30,132,242,0.52),
    0 0 7px rgba(30,132,242,0.92),
    0 0 11px rgba(30,132,242,0.78),
    0 0 16px rgba(30,132,242,0.92);
}

@keyframes neon {
  from {
    text-shadow:
    0 0 6px rgba(224,202,227,0.98),
    0 0 30px rgba(224,202,227,0.34),
    0 0 12px rgba(242,29,129,0.52),
    0 0 22px rgba(242,29,129,0.92),
    0 0 38px rgba(242,29,129,0.78),
    0 0 60px rgba(242,29,129,0.92);
  }
  to {
    text-shadow:
    0 0 6px rgba(224,202,227,0.98),
    0 0 30px rgba(224,202,227,0.42),
    0 0 12px rgba(242,29,129,0.58),
    0 0 22px rgba(242,29,129,0.84),
    0 0 38px rgba(242,29,129,0.88),
    0 0 60px rgba(242,29,129,1);
  }
}
</style>

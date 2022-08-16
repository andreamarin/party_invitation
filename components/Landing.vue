<template>
  <div class="invitation invite-image">
    <div class="title-container">
      <span class="title title-pink-neon">
        ¡Mi cumpleaños 60!
      </span>
    </div>
    <div class="subtitle-container">
      <span class="subtitle">
        Acompáñame este 8 de octubre a festejar en grande
      </span>
    </div>
    <!-- TODO: flecha de detalles -->
  </div>
</template>

<script>

export default {}
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
  width: 90%;
  text-align: center;
}
.title{
  font-family: var(--title-font);
  color: #FFADFE;
  font-size: 7vh;
}
.subtitle-container{
  width: 80%;
  text-align: center;
  margin-top: 60px;
}
.subtitle{
  color: var(--light-shades);
  font-size: 3vh;
  font-family: var(--subtitle-font);
}
.title-pink-neon {
  text-shadow:
    0 0 3px rgba(255,194,254,0.98),
    0 0 30px rgba(255,194,254,0.34),
    0 0 12px rgba(255,10,251,0.52),
    0 0 22px rgba(255,10,251,0.92),
    0 0 38px rgba(255,10,251,0.78),
    0 0 60px rgba(255,10,251,0.92);
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

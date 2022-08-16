<template>
  <div class="invitation invite-image">
    <div class="title-container">
      <span class="title pink-neon-text">
        Bienvenida a los 60
      </span>
    </div>
    <div class="subtitle-container">
      <span class="subtitle">
        ¡vamos a festejar en grande mi cumpleaños este <span class="text-highlight">8 de octubre</span>!
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
  font-size: 6vh;
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

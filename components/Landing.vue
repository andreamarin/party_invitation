<template>
  <div class="invitation">
    <div class="title-container">
      <span class="title">
        Mis 60!
      </span>
    </div>
    <div class="subtitle-container">
      <span class="subtitle">
        8 de octubre de 2022
      </span>
    </div>
  </div>
</template>

<script>
export default {

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
  color: var(--main-color);
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
</style>

<template>
  <div class="location-card">
    <span class="location-title">
      Dónde?
    </span>
    <div class="location-data">
      <div class="location-info">
        <span class="venue-name">
          Salón Gaudí
        </span>
        <span class="address">
          GRUPO FORESTA Av Constituyentes 800
          <br>Lomas Altas, Miguel Hidalgo, 11100
          <br>Ciudad de México, CDMX
        </span>
        <span class="time">
          Sábado 8 de octubre, 14:00hrs
        </span>
      </div>
      <div class="location-map-container">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d481916.13184181333!2d-99.69946251598604!3d19.327117594292908!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85d201a4d5256331%3A0xcd24100d00151cf0!2zU2Fsw7NuIEdhdWTDrS4!5e0!3m2!1sen!2smx!4v1660194035288!5m2!1sen!2smx"
          class="venue-map"
          allowfullscreen=""
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style>
.location-card {
    height: 90%;
    width: 80%;
    padding: 30px;
    border-radius: 25px;
    background-color: var(--dark-shades);
}
.location-title{
  font-family: var(--title-font);
  color: var(--main-color);
  font-size: 9vw;
}

.venue-name {
  padding-right: 10px;
  color: var(--light-accent);
  font-family: var(--subtitle-font);
  font-size: 5vh;
  margin-block-start: 30px;
  margin-block-end: 10px;
}

.address {
  padding-right: 10px;
  color: var(--light-shades);
  font-size: 2vh;
}

.time {
  padding-right: 10px;
  color: var(--light-accent);
  font-family: var(--subtitle-font);
  font-size: 3vh;
  margin-block-start: 40px;
}

.location-info{
  display: flex;
  flex-direction: column;
}

.location-data{
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: space-between;
  column-gap: 100px;
  row-gap: 60px;
}

.location-map-container{
  /* align self */
  flex-grow: 2;

  /* align child items */
  display: flex;
  flex-direction: row;
  justify-content: center;
}

.venue-map {
  border: 0;
  min-height: 300px;
  width: 100%;
}

</style>

<template>
  <!-- <div class="location"> -->
  <div class="location-card">
    <div class="location-content">
      <span class="title">
        Dónde?
      </span>
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
      <div class="mapouter">
        <div class="gmap_canvas">
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3763.361588132718!2d-99.2236461!3d19.396776799999994!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85d201a4d5256331%3A0xce3c255b7ca419e5!2sForesta!5e0!3m2!1sen!2smx!4v1660144663003!5m2!1sen!2smx"
            width="600"
            height="450"
            style="border:0;"
            allowfullscreen=""
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          />
          <!-- <iframe
            id="gmap_canvas"
            width="600"
            height="500"
            src="https://maps.google.com/maps?q=Salon%20Gaud%C3%AD,%20Av%20Constituyentes%20800&t=&z=15&ie=UTF8&iwloc=&output=embed"
            frameborder="0"
            scrolling="no"
            marginheight="0"
            marginwidth="0"
          /> -->
        </div>
      </div>
    </div>
  </div>
  <!-- </div> -->
</template>

<script>
export default {
}
</script>

<style>
.location {
    height: 100%;
    width: 100%;
    align-content: center;
}
.location-card {
    margin-left: 40px;
    margin-right: 40px;
    height: 100%;
    width: 100%;
    padding: 30px;
    border-radius: 25px;
    background-color: var(--dark-shades);
}
.location-content{
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
  justify-content: baseline;
}
.venue-name {
  padding-right: 10px;
  color: var(--light-accent);
  font-family: var(--subtitle-font);
  font-size: 2rem;
  margin-block-start: 30px;
  margin-block-end: 10px;
}
.address {
  padding-right: 10px;
  color: var(--light-shades);
  font-size: 1.3rem;
}
.time {
  padding-right: 10px;
  color: var(--light-accent);
  font-family: var(--subtitle-font);
  font-size: 1.5rem;
  margin-block-start: 40px;
}
.mapouter{
  position:relative;
  text-align:right;
  height:500px;
  width:600px;
}
.gmap_canvas {
  overflow:hidden;
  background:none!important;
  height:500px;
  width:600px;
}
</style>

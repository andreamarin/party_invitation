<template>
  <div class="card ceremony-card">
    <div class="ceremony-data">
      <div class="ceremony-info">
        <span class="card-subtitle party-invite">
          ¡Acompáñame a festejar mis <span class="age-highlight">32</span> años en mi casa!
        </span>

        <span class="card-data information">
          También se llevará a cabo una misa para festejar y recordar a mi abuelo <span class="name-highlight">Leandro Medina</span> y a mi tío <span class="name-highlight">Alejandro Pérez</span>.
        </span>
        <!-- <div class="name-container">
          <span class="card-subtitle people-name">
            Leandro Medina
          </span>
          <span class="card-data address center">
            y
          </span>
          <span class="card-subtitle people-name">
            Alejandro Perez
          </span> -->
      </div>
      <div class="address-container">
        <span class="card-subtitle-small venue-name">
          Rectoría Santa Teresa de Avila
        </span>
        <span class="card-subtitle-small venue-name">
          18:00 hrs
        </span>
        <span class="card-data-small address">
          Arcos Ote. 285
          <br>Jardines del Sur, Xochimilco, 16050
          <br>Ciudad de México, CDMX
        </span>
        <div class="location-map-container">
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3766.5978552478464!2d-99.1159388!3d19.256350299999998!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85ce014f50615b81%3A0x53ebf6c5b3b0f1d6!2sRector%C3%ADa%20Santa%20Teresa%20de%20Avila!5e0!3m2!1sen!2smx!4v1676840978224!5m2!1sen!2smx"
            class="venue-map"
            allowfullscreen=""
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          />
        </div>
      </div>
      <span class="card-data information">
        P.D. La dirección de mi casa ya la conocen ;)
      </span>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

  <style>
  .ceremony-card {
      /* background-color: var(--yellow-main-color); */
      background-color: var(--dark-accent);
  }

  .ceremony-info{
    display: flex;
    flex-direction: column;
  }

  .ceremony-data{
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: space-between;
    column-gap: 100px;
    row-gap: 40px;
  }

  .center{
    margin: auto;
  }

  .name-container{
    margin-top: 20px;
    margin-bottom: 50px;
  }

  .party-invite{
    padding-right: 10px;
    color: var(--wine-main-color);
    font-family: var(--subtitle-font);
    margin-bottom: 30px;
    text-align: center;
  }

  .name-highlight {
    color: var(--dark-shades);
    font-family: var(--subtitle-font);
    font-size: 2.6vh;
  }

  .information {
    padding-right: 10px;
    color: var(--light-shades);
  }

  .address-container {
    display: flex;
    flex-direction: column;
    width: 100%;
  }

  .venue-name {
    color: var(--dark-shades);
  }

  .address {
    padding-right: 10px;
    color: var(--light-shades);
    margin-top: 8px;
    margin-bottom: 20px;
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

  @media only screen and (min-width: 768px) {
    .venue-map {
      border: 0;
      min-height: 300px;
      width: 100%;
    }
  }

  </style>

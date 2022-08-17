<template>
  <a v-scroll-to="href" href="#" class="arrow-link">
    <div class="arrow-containter">
      <svg class="arrow-svg shadow">
        <path class="arrow" d="M 0 0 L 30 20 L 60 0" />
      </svg>
    </div>
    <div class="details-text">
      Detalles
    </div>
  </a>
</template>

<script>
export default {
  props: {
    href: {
      type: String,
      default: '#'
    }
  }
}
</script>

<style>

.arrow-link{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    text-decoration: none;
}

.arrow{
    fill: transparent;
    stroke: var(--main-color);
    stroke-width: 2px;
}

.arrow-svg {
    display: block;
    height: 100%;
    width: 100%;
    animation: jumpInfinite 1.5s infinite;
}

.shadow{
    -webkit-filter:
        drop-shadow(0px 0px 2px #F30AFF)
        drop-shadow(0px 0px 5px #F30AFF)
        drop-shadow(0px 0px 10px #F30AFF)
    ;
    filter:
        drop-shadow(0px 0px 2px #F30AFF)
        drop-shadow(0px 0px 5px #F30AFF)
        drop-shadow(0px 0px 10px #F30AFF)
    ;
}

.arrow-containter {
    height: 40px;
    width: 60px;
}

.details-text{
    color: #FFD6FF;
    font-family: 'Synonym-Regular';
    font-size: 1.6vh;

    text-shadow:
    0 0 3px rgba(255,194,254,0.98),
    0 0 30px rgba(255,194,254,0.34),
    0 0 12px rgba(255,10,251,0.52),
    0 0 22px rgba(255,10,251,0.92),
    0 0 38px rgba(255,10,251,0.78);
}

@keyframes jumpInfinite {
  0% {
    margin-top: 0;
  }
  50% {
    margin-top: 10px;
  }
  100% {
    margin-top: 0;
  }
}
</style>

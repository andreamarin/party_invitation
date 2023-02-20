<template>
  <a v-scroll-to="href" href="#" class="arrow-link">
    <div class="arrow-containter">
      <svg class="arrow-svg shadow">
        <path class="arrow" d="M 0 0 L 30 20 L 60 0" />
      </svg>
      <!-- <svg class="arrow-svg shadow">
        <path class="arrow" d="M 0 0 L 30 20 L 60 0" />
      </svg> -->
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
    stroke: var(--yellow-main-color);
    stroke-width: 2px;
}

.arrow-svg {
    display: block;
    height: 100%;
    width: 100%;
    animation: jumpInfinite 1.5s infinite;
}

/* .shadow{
    -webkit-filter:
        drop-shadow(0px 0px 2px #68FFFF)
        drop-shadow(0px 0px 5px #68FFFF)
        drop-shadow(0px 0px 10px #68FFFF)
    ;
    filter:
        drop-shadow(0px 0px 2px #68FFFF)
        drop-shadow(0px 0px 5px #68FFFF)
        drop-shadow(0px 0px 10px #68FFFF)
    ;
} */

.arrow-containter {
    height: 40px;
    width: 60px;
}

.details-text{
    font-family: var(--body-font);
    color: var(--yellow-main-color);
    font-size: 2vh;
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

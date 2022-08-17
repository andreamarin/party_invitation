<template>
  <div class="goodbye">
    <div class="goodbye-container">
      <span class="title goodbye-phrase pink-neon-text">
        ¡Te esperamos!
      </span>
    </div>
  </div>
</template>

<script>

export default {
}
</script>

<style>
.goodbye {
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  /* background-blend-mode: hard-light;
  background-image:
  url('@/assets/dark_background.jpg'),
  radial-gradient(circle, #7277d5, #696fd3, #6166d0, #585ece, #4f55cb, #4a50c7, #444ac4, #3f45c0, #3c42bb, #3a3fb6, #373db2, #343aad) */
  /* radial-gradient(circle, #262a7e, #242878, #222672, #20246c, #1e2266, #1c2060, #1b1e59, #191c53, #171a4b, #141744, #12153c, #101235) */
  /* ; */
}

.goodbye-container{
  width: 80%;
  text-align: center;
  margin-bottom: 40px;

}

.goodbye-phrase{
  animation:
    blink 8s infinite;
}

@keyframes neon-flicker {
  from {
    text-shadow:
    0 0 6px rgba(255,194,254,0.92),
    0 0 30px rgba(255,194,254,0.34),
    0 0 12px rgba(255,10,251,0.52),
    0 0 21px rgba(255,10,251,0.92),
    0 0 34px rgba(255,10,251,0.78),
    0 0 54px rgba(255,10,251,0.92);
  }
  to {
    text-shadow:
    0 0 6px rgba(255,194,254,0.98),
    0 0 30px rgba(255,194,254,0.42),
    0 0 12px rgba(255,10,251,0.58),
    0 0 22px rgba(255,10,251,0.84),
    0 0 38px rgba(255,10,251,0.88),
    0 0 60px rgba(255,10,251,1);
  }
}

@keyframes blink {
  20%,
  24%,
  55% {
    color: #111;
    text-shadow: none;
  }

  0%,
  19%,
  21%,
  23%,
  25%,
  54%,
  56%,
  100% {
  text-shadow:
    0 0 6px rgba(255,194,254,0.98),
    0 0 30px rgba(255,194,254,0.42),
    0 0 12px rgba(255,10,251,0.58),
    0 0 22px rgba(255,10,251,0.84),
    0 0 38px rgba(255,10,251,0.88),
    0 0 60px rgba(255,10,251,1);
    color: #FFADFE;
  }
}

</style>

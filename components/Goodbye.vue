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
}

.goodbye-container{
  width: 80%;
  text-align: center;
  margin-bottom: 40px;

}

.goodbye-phrase{
  animation:
    blink 12s infinite;
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

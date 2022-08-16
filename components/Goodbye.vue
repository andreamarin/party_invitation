<template>
  <div class="goodbye">
    <div class="goodbye-container">
      <span class="title goodbye-phrase pink-neon-text">
        ¡Te esperamos!
      </span>
    </div>
    <boombox />
  </div>
</template>

<script>
import Boombox from './Boombox.vue'

export default {
  components: { Boombox }
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
  color: var(--light-accent-2);
}

</style>

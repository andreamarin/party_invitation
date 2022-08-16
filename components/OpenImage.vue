<template>
  <div class="modal-wrapper" @click="$emit('close-modal')">
    <img :src="imagePath" class="full-image">
  </div>
</template>

<script>
export default {
  name: 'OpenImage',
  props: {
    imagePath: {
      type: String,
      default: 'path'
    }
  }
}
</script>

<style>
  .modal-wrapper {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(17, 2, 39, 0.9);

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .full-image {
    max-height: 70%;
  }

</style>

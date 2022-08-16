<template>
  <div>
    <div class="outfit-image" :style="imageStyle" @click="showImage=true" />
    <open-image v-if="showImage" :image-path="imagePath" @close-modal="showImage=false" />
  </div>
</template>

<script>
import OpenImage from '@/components/OpenImage.vue'

export default {
  components: {
    OpenImage
  },
  props: {
    imageName: {
      type: String,
      default: 'foto'
    },
    imagePath: {
      type: String,
      default: 'path'
    }
  },
  data () {
    return {
      showImage: false
    }
  },
  computed: {
    imageStyle () {
      return {
        backgroundImage: 'url(' + this.imagePath + ')'
      }
    }
  }
}
</script>

<style>
.outfit-image{
  overflow: clip;
  border-radius: 4px;
  background-size: cover;
  background-position: center;
  width: 200px;
  height: 200px;
  margin: 5px;
}
</style>

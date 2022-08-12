<template>
  <div class="images-container">
    <outfit-image v-for="image in chosenImages" :key="image.imageName" :image-name="image.imageName" :image-path="image.imagePath" />
    <!-- <masonry-wall :items="chosenImages" :column-width="300" :gap="5">
      <template v-slot:default="{item}">
        <outfit-image :image-name="item.imageName" :image-path="item.imagePath" />
      </template>
    </masonry-wall> -->
  </div>
</template>

<script>
import OutfitImage from '@/components/OutfitImage.vue'
export default {
  components: {
    OutfitImage
  },
  data () {
    return {
      outfitFiles: [],
      chosenImages: [],
      numImages: 16
    }
  },
  mounted () {
    this.getImages(require.context('../assets/outfits/', true, /\.(png|jpg|webp)$/))
    this.chooseRandomImages()

    // refresh images every 10s
    // this.timer = setInterval(this.chooseRandomImages, 10000)
  },
  methods: {
    getImages (r) {
      r.keys().forEach(key => (this.outfitFiles.push({ imagePath: r(key), imageName: key })))
    },
    chooseRandomImages () {
      const images = []
      if (this.outfitFiles.length > 0) {
        const possibleChoices = [...this.outfitFiles]
        for (let i = 0; i < this.numImages; i++) {
          // get random index
          const randomIndex = Math.floor(Math.random() * possibleChoices.length)
          images.push(possibleChoices[randomIndex])

          // remove choice from list
          possibleChoices.splice(randomIndex, 1)
        }
        this.chosenImages = images
      }
    }
  }
}
</script>

<style>
.images-container {
  width: 80%;
  display: flex;
  direction: row;
  flex-wrap: wrap;
}

</style>

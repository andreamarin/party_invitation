<template>
  <div class="card dress-code-card large-blue-neon-box">
    <span class="card-title dress-code-title">
      ¿Cómo tengo que ir?
    </span>
    <span class="card-data dress-code-info">
      Es una fiesta <span class="text-highlight">temática de los 80</span>, te invito a vestirte al estilo de la época.
    </span>
    <span class="card-data dress-code-info">
      Aquí hay unas fotos para inspirarte (dale click a una para verla más grande).
    </span>
    <div class="images-container">
      <outfit-image v-for="image in chosenImages" :key="image.imageName" :image-name="image.imageName" :image-path="image.imagePath" />
    </div>
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
.dress-code-card {
    /* background-color: var(--blue-main-color); */

    display: flex;
    flex-direction: column;
}

.dress-code-title{
  color: var(--blue-main-color);
}

.dress-code-info{
  margin-top: 20px;
  color: var(--light-shades);
}

.images-container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  margin-left: auto;
  margin-right: auto;
  margin-top: 40px;
  width: 100%;
}

.text-highlight {
  font-family: var(--subtitle-font);
  color: var(--pink-main-color);
}

@media only screen and (min-width: 768px) {
  .images-container{
    width: 95%;
    padding: 20px;
  }
}

</style>

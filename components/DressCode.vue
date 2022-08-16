<template>
  <div class="dress-code-card">
    <span class="dress-code-title">
      Cómo tengo que ir?
    </span>
    <span class="dress-code-info">
      Es una fiesta <span class="text-highlight">temática de los 80</span>, te invito a vestirte al estilo de la época.
    </span>
    <span class="dress-code-info">
      Aquí hay unas fotos para inspirarte
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
    height: 90%;
    width: 80%;
    padding: 30px;
    border-radius: 25px;
    background-color: var(--light-accent);

    display: flex;
    flex-direction: column;
}

.dress-code-title{
  font-family: var(--title-font);
  color: var(--dark-shades);
  font-size: 9vw;
}

.dress-code-info{
  color: var(--light-shades);
  font-size: 2.6vh;
  margin-top: 20px;
  margin-left: 15px;
}

.images-container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  margin: auto;
  width: 95%;
  padding: 20px;
}

.text-highlight {
  font-family: var(--subtitle-font);
  color: var(--dark-accent);
}

</style>

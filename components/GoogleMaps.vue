<template>
  <div>
    <div ref="mapa" class="mapa" />
    <template v-if="Boolean(google) && Boolean(map)">
      <slot :google="google" :map="map" />
    </template>
  </div>
</template>

<script>
import GoogleMapsApiLoader from 'google-maps-api-loader'

export default {
  props: {
    mapConfig: Object,
    apiKey: String
  },

  data () {
    return {
      google: null,
      map: null
    }
  },

  async mounted () {
    const googleMapApi = await GoogleMapsApiLoader({
      apiKey: this.apiKey
    })
    this.google = googleMapApi
    this.initializeMap()
  },

  methods: {
    initializeMap () {
      const mapContainer = this.$refs.mapa
      this.map = new this.google.maps.Map(mapContainer, this.mapConfig)
    }
  }
}
</script>

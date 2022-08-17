
<template>
  <div class="arrows-main-container">
    <scroll-down-arrow />
  </div>
</template>

<script>
import ScrollDownArrow from '@/components/ScrollDownArrow'

export default {
  components: {
    ScrollDownArrow
  },
  head: {
    bodyAttrs: {
      class: 'main-body'
    }
  }
}
</script>

<style>
.arrows-main-container{
    display: flex;
    flex-direction: column;
    justify-content: center;
    /* padding: 40px; */
}
</style>

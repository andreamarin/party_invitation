<template>
  <div class="question-container">
    <div class="faq-question">
      <b class="q-icon">Q.</b>{{ question }}
    </div>
    <div class="faq-answer">
      {{ answer }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'OpenImage',
  props: {
    question: {
      type: String,
      default: 'cuando es?'
    },
    answer: {
      type: String,
      default: 'hoy'
    }
  }
}
</script>

<style>
.question-container{
    padding-left: 20px;
    padding-right: 10px;
    padding-top: 20px;
    padding-bottom: 20px;
    margin-bottom: 10px;
}
.faq-question{
    font-family: var(--subtitle-font);
    color: var(--main-color);
    font-size: 3.5vh;

    margin-bottom:6px;
    position: relative;
    padding-left: 50px;
}

.faq-answer{
    color: var(--dark-shades);
    font-size: 2.8vh;
    padding-left: 50px;
}

.q-icon{
    position: absolute;
    left: 0;
}

</style>

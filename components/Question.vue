<template>
  <div class="question-container">
    <div class="card-subtitle faq-question">
      <b class="q-icon">Q.</b>{{ question }}
    </div>
    <div class="card-data faq-answer">
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
    padding-top: 20px;
    padding-bottom: 20px;
}
.faq-question{
    color: var(--light-accent);

    margin-bottom:6px;
    position: relative;
    padding-left: 40px;
}

.faq-answer{
    color: var(--light-shades);
    padding-left:40px;
}

.q-icon{
    position: absolute;
    left: 0;
}

@media only screen and (min-width: 768px) {
  .question-container{
    padding-left: 20px;
    padding-right: 10px;
    margin-bottom: 10px;
  }

  .faq-question{
    padding-left: 50px;
  }

  .faq-answer{
    padding-left: 50px;
  }

}

</style>

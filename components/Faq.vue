<template>
  <div class="faq-card">
    <span class="faq-title">
      Preguntas
    </span>
    <div class="faq-questions">
      <question
        v-for="(question, index) in questions"
        :key="index"
        :question="question.q"
        :answer="question.a"
      />
    </div>
  </div>
</template>

<script>
import Question from '@/components/Question.vue'

export default {
  components: {
    Question
  },
  data () {
    return {
      questions: [
        { q: 'Habrá comida?', a: 'Sí, se va a dar una comida de cuatro tiempos' },
        { q: 'Tengo que llevar algo?', a: 'En el evento hay barra libre, sin embargo puedes traer la botella de tu preferencia. El descorche es libre.' },
        { q: 'Qué mezcladores hay?', a: 'Los mezcladores usuales (coca, manzana, agua mineral, ...) y agua quina' }
      ]

    }
  }
}
</script>

<style>
.faq-card {
    height: 90%;
    width: 80%;
    padding: 30px;
    border-radius: 25px;
    background-color: var(--light-shades);

    display: flex;
    flex-direction: column;
}

.faq-title{
  font-family: var(--title-font);
  color: var(--dark-accent);
  font-size: 9vw;
}

.faq-questions{
  width: 95;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

</style>

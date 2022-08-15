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
    <div>
      Si tienes alguna duda adicional por favor contacta a Mario Medina (+52 55...) o a Laura Monroy (+52 55...)
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
        { q: 'Habrá comida?', a: 'Sí, a las 14:00 se servirá la comida.' },
        { q: 'Cuentan con menú infantil/vegetariano?', a: 'Sí hay alternativas infantil y vegetariana pero solo bajo pedido. Te pedimos nos avises lo antes posible si lo requieres.' },
        { q: 'Qué habrá de tomar?', a: 'Refrescos, agua mineral, agua tónica y además, el salón ofrece barra libre nacional (tequila, ron, whisky, vodka y brandy).' },
        { q: 'Habrá descorche libre?', a: 'Sí, puedes llevar el alcohol adicional que gustes, siempre y cuando sean botellas marbetadas.' },
        { q: 'A qué hora termina el salón?', a: 'La fiesta en el salón acaba a las 19:00 hrs' },
        { q: 'Hay estacionamiento?', a: 'Sí, el salón cuenta con el servicio adicional de valet parking.' },
        { q: 'Hay fecha límite para confirmar mi asistencia?', a: 'Por favor avísanos a más tardar el 8 de septiembre para que podamos tener un conteo preciso.' },
        { q: 'Puedo apoyar en algo?', a: 'Participando al máximo en el evento y una gran actitud para hacer de este, el mejor cumpleaños' }
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

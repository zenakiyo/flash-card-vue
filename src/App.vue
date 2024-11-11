<script setup>
import qandaCard from './components/qandaCard.vue';
const data = [
  {
    id: 3457,
    question: 'What language is React based on?',
    answer: 'JavaScript',
  },
  {
    id: 7336,
    question: 'What are the building blocks of React apps?',
    answer: 'Components',
  },
  {
    id: 8832,
    question: "What's the name of the syntax we use to describe a UI in React?",
    answer: 'JSX',
  },
  {
    id: 1297,
    question: 'How to pass data from parent to child components?',
    answer: 'Props',
  },
  {
    id: 9103,
    question: 'How to give components memory?',
    answer: 'useState hook',
  },
  {
    id: 2002,
    question: 'What do we call an input element that is completely synchronised with state?',
    answer: 'Controlled element',
  },
]
</script>

<template>
  <div class="container">
    <qandaCard v-for="i in data" :key="i.id" :data = "i"/>
  </div>
</template>

<style scoped>

.container {
  width: 100%;
  height: 95vh;
  display: grid;
  grid-template-columns: repeat(4, auto);
  justify-content: space-evenly;
  align-items: center;
  gap: auto;
}
</style>

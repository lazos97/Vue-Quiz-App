<script setup>
import { defineProps } from 'vue'
import { RouterLink } from 'vue-router'

const {} = defineProps(['quizQuestionLength', 'numberOfCorrectAnswers'])
</script>

<template>
  <div class="results">
    <p>Your results...</p>
    <h1>{{ numberOfCorrectAnswers }} / {{ quizQuestionLength }}</h1>
    <RouterLink class="backBtn" to="/">Go back</RouterLink>
  </div>
</template>

<style scoped>
.results {
  text-align: center;
  padding: 100px 0px;
}

p {
  font-size: 25px;
}

h1 {
  font-size: 80px;
}

.backBtn {
  text-decoration: none;
  font-size: 20px;
  font-style: italic;
  font-weight: bold;
  background-color: black;
  color: white;
  padding: 5px;
  border-radius: 5px;
}
</style>

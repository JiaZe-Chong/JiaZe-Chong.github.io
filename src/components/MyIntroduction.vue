<script setup>
import { ref } from 'vue'
const det = ref(false)
</script>

<template>
  <div class="item">
    <h1>Introduction:</h1>
    <p>
      I am a computer science student passionate and curious about everything computer science, from
      artificial intelligence and machine learing to low-level embedded software. I am doing
      extremely well in my academics and would like to put the things I learnt in class to use. I am
      currently working as a lab research assistant involved in software engineering and problem
      solving.
    </p>
    <p>Contact me if you are interested to know more about me.</p>
    <button class="btn" @click="det = !det">Relevant Courses</button>
    <div v-show="det" class="detail">
      <p>-Data Structures</p>
      <p>-Software Development</p>
      <p>-Advanced Programming Techniques</p>
      <p>-Database Management Systems</p>
      <p>-Algorithms</p>
      <p>-Programming Languages</p>
    </div>
  </div>
</template>

<style scoped>
.btn {
  color: #fff;
  background: linear-gradient(315deg, #42d392 25%, #647eff);
  border: none;
  padding: 5px 10px;
  margin: 5px;
  border-radius: 8px;
  cursor: pointer;
}

.detail {
  width: 90%;
  left: 5%;
}
h1 {
  color: hsla(160, 100%, 37%, 1);
}
</style>

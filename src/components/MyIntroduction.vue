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
      extremely well academically and would like to put the things I learnt in practice. I am
      currently working as a software engineering intern at Ag Leader Technology involving guidance
      and steering systems. I am actively looking for a full time job after graduation.
    </p>
    <p>Feel free to reach out if you are interested to know more about me or what I do.</p>
    <button class="btn" @click="det = !det">Relevant Courses</button>
    <div v-show="det" class="detail">
      <p>-Data Structures</p>
      <p>-Software Development</p>
      <p>-Advanced Programming Techniques</p>
      <p>-Database Management Systems</p>
      <p>-Algorithms</p>
      <p>-Programming Languages</p>
      <p>-Operating Systems</p>
      <p>-Algorithms for Large Data Sets</p>
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

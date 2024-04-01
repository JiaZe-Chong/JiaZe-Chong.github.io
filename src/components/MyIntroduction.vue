<script setup>
import { ref } from 'vue'
const det = ref(false)
</script>

<template>
  <div class="item">
    <h1>Introduction:</h1>
    <p>
      I am a computer science student who is passionate and curious about everything computer
      science, from artificial intelligence and machine learning to low-level embedded software. I have excelled academically and would like to apply the knowledge I've gained. I
      work as a software engineering intern at Ag Leader Technology, involving guidance and steering
      systems. I am actively looking for a full-time job after graduation.
    </p>
    <p>Please let me know if you'd like to learn more about me or what I do.</p>
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
      <p>Software System Safety</p>
      <p>Principle of Artificial Intelligence</p>
      <p>Network Protocol and Security</p>
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

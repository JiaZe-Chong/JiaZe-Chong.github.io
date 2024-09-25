<script setup>
import { ref } from 'vue'
const det = ref(false)
</script>

<template>
  <div class="item">
    <h1>Introduction:</h1>
    <p>
      Highly skilled Software Engineer with over 2 years of experience in software development using
      C++. Proficient in Agile and Scrum methodologies, with a strong ability to learn and adapt to
      new technologies. Demonstrated competence in both independent and collaborative work
      environments. Proven track record in developing self-driving software solutions, enhancing
      user interfaces, and engineering advanced path-planning features. Adept at boosting test
      coverage and creating innovative guidance systems. Holds a B.S. in Computer Science, Summa Cum
      Laude, from Iowa State University.
    </p>
    <p>Please let me know if you'd like to learn more about me or what I do.</p>
    <button class="btn" @click="det = !det">Courses Taken</button>
    <div v-show="det" class="detail">
      <p>-Data Structures</p>
      <p>-Software Development</p>
      <p>-Advanced Programming Techniques</p>
      <p>-Database Management Systems</p>
      <p>-Algorithms</p>
      <p>-Programming Languages</p>
      <p>-Operating Systems</p>
      <p>-Algorithms for Large Data Sets</p>
      <p>-Software System Safety</p>
      <p>-Principle of Artificial Intelligence</p>
      <p>-Network Protocol and Security</p>
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

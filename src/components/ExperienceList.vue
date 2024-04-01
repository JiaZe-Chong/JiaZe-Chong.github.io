<script setup>
import ExperienceItem from './ExperienceItem.vue'
</script>

<template>
  <div class="item">
    <h1>Work Experience:</h1>

    <ExperienceItem>
      <template #title> Software Engineering Intern at Ag Leader Technology </template>

      <template #introduction>
        Developed and maintained software for vehicle displays, specializing in guidance systems.
      </template>

      <template #details>
        <p>-Language: <span>C++</span></p>
        <p>-Library/Technology: <span>Qt</span></p>
        <p>-Utilized event-driven architecture for cross-thread communication.</p>
        <p>-Utilized Qt's slots and signals for cross-object communication.</p>
        <p>-Developed and maintained unit tests run using Ctest.</p>
        <p>
          -Biggest lesson: Knowing when to ask for help. You don't want to immediately ask for help
          when you see a problem, but at the same time, you don't want to be stuck on it for an
          extended period of time.
        </p>
      </template>
    </ExperienceItem>

    <ExperienceItem>
      <template #title> Lab Research Assistant at Iowa State University </template>

      <template #introduction>
        Developed and maintained programs utilizing multiple libraries to control imaging
        technologies such as cameras and profilers to look for surface anomalies.
      </template>

      <template #details>
        <p>-Language: <span>C</span>, <span>C++</span></p>
        <p>-Library/Technology: <span>Pylon Software Suite</span></p>
        <p>
          -Utilized analog signals to enable communication between imaging technologies and Cobots.
        </p>
        <p>-Utilized memory manipulation to allow efficient splitting and merging of images.</p>
        <p>-Developed and maintained documentation to guide the team in developing programs.</p>
        <p>
          -Biggest lesson: Documentation, how reading documentation is one of the most important
          step before writing any code, and how writing useful documentation helps maintainance
        </p>
      </template>
    </ExperienceItem>
  </div>
</template>

<style scoped>
h1 {
  color: hsla(160, 100%, 37%, 1);
}

span {
  font-weight: bold;
}
</style>

<script setup>
import ExperienceItem from './ExperienceItem.vue'
</script>

<template>
  <div class="item">
    <h1>Work Experience:</h1>
    <ExperienceItem>
      <template #title> Lab Research Assistant at Iowa State University </template>

      <template #introduction>
        Developed and maintained C++ programs to control utilizing multiple libraries to control
        imaging technologies such as cameras and profilers to look for surface anomalies.
      </template>

      <template #details>
        <p>-Language: C, C++</p>
        <p>-Library/Technology: Pylon Software Suite</p>
        <p>
          -Developed programs written in C++ and “Block Coding” for communication between imaging
          technologies and a robot arm via different voltages.
        </p>
        <p>-Wrote scripts in C to assist communication between different technologies.</p>
        <p>
          -Developed an executable in C++ that allows people to control the camera's settings and
          capture images.
        </p>
        <p>
          -Developed software documentation to guide the team in developing programs by breaking
          large objectives into smaller tasks.
        </p>
        <p>
          -Developed a utility program in C that stitches 40 images into 1 large image and breaks up
          1 large image into 297 smaller images using memory manipulation to help with analysis.
        </p>
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
</style>

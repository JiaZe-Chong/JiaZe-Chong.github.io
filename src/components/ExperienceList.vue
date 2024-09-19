<script setup>
import ExperienceItem from './ExperienceItem.vue'
</script>

<template>
  <div class="item">
    <h1>Work Experience:</h1>

    <ExperienceItem>
      <template #title> Software Engineer at Ag Leader Technology </template>

      <template #introduction>
        Developed and maintained software for vehicle displays, specializing in guidance systems.
      </template>

      <template #details>
        <p>-Language: <span>C++</span></p>
        <p>-Library/Technology: <span>Qt</span></p>
        <p>
          -Developed self-driving software solutions for agricultural vehicles, automating critical
          maneuvers.
        </p>
        <p>
          -Engineered an advanced path planning feature for complex navigation beyond simple turns.
        </p>
        <p>-Enhanced user interface for next-generation displays, improving user experience.</p>
        <p>
          -Created proof of concept (POC) and minimal viable product (MVP) for innovative guidance
          systems leveraging implement location.
        </p>
        <p>
          -Collaborated with product owners, stakeholders, and testers to communicate vital
          decision-making processes.
        </p>
        <p>
          -Boosted test coverage for display and guidance system code, ensuring higher reliability.
        </p>
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
          -Designed and developed imaging systems for capturing high-resolution images to detect
          surface anomalies.
        </p>
        <p>
          -Innovated low-cost solutions for high-resolution imaging through image stitching
          techniques.
        </p>
        <p>
          -Implemented and evaluated post-processing methods to enhance surface anomaly detection.
        </p>
        <p>
          -Developed communication protocols between imaging systems and Cobot arms for automated
          camera movement.
        </p>
        <p>
          -Maintained comprehensive documentation to support system development and user guidance.
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

span {
  font-weight: bold;
}
</style>

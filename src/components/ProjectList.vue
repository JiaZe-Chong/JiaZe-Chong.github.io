<script setup>
import ExperienceItem from './ExperienceItem.vue'
</script>

<template>
  <h1>Projects:</h1>

  <ExperienceItem
    :points="[
      'Used conditional rendering to only show details on click.',
      'Utilized components to organize code base.',
      'Used slots and props to pass data into components.',
      'Language: Javascript',
      'Library/Technology: VueJS, Github Pages',
      'Biggest lesson: You can never really learn everything there is to learn about some language/framework/library. You just need to learn the fundamental and keep learning while you are using it.'
    ]"
  >
    <template #title> About Me(this) </template>

    <template #introduction>
      A webpage that introduces myself along with the projects and work experiences I have.
    </template>
  </ExperienceItem>

  <ExperienceItem
    :points="[
      'Used nCurses for terminal manipulation and unbuffered input.',
      'Developed and used a parser to parse data from a CSV file.',
      'Utilized object-oriented programming to simplify and streamline the development of the game.',
      'Utilized header files and Makefile to improve code maintainability.',
      'Language: C and C++',
      'Library/Technology: nCurses, Makefile',
      'Biggest lesson: Technical dept, what seems like an easy solution for current complication may lead to a much harder problem that needs to be solve, so always plan ahead.'
    ]"
  >
    <template #title> Pokemon Game </template>

    <template #introduction>
      A Pokemon game with the core gameplay such as random map generation, player movement, random
      occuring events, and combat system implemented.
    </template>
  </ExperienceItem>

  <ExperienceItem
    :points="[
      'HTTP requests and WebSockets are used for communication between the front-end client and the back-end server. ',
      'Implemented CRUD functions using REST API to manipulate data stored in the back-end server.',
      'Utilized fragments and activities to make UI more friendly.',
      'Language: Java',
      'Library/Technology: Android Studio, Springboot, Git',
      'Biggest lesson: Plan ahead, as projects get bigger, it is very important to plan ahead as even the simplest things such as naming variables can be hard due to namespace pollution.'
    ]"
  >
    <template #title> Driveway </template>

    <template #introduction>
      An Android application that allows users rent parking spots.
    </template>
  </ExperienceItem>
</template>

<style scoped>
h1 {
  color: hsla(160, 100%, 37%, 1);
}
</style>

<script setup>
import ExperienceItem from './ExperienceItem.vue'
</script>

<template>
    <h1>Projects:</h1>
    <ExperienceItem :points="['Language: C and C++', 'Library/Technology: nCurses, Makefile']">
      <template #title> Pokemon Game </template>

      <template #introduction>
        A Pokemon game with the core gameplay such as random map generation, player movement, random occuring events, and combat system implemented.
      </template>
    </ExperienceItem>

    <ExperienceItem :points="['Language: Java', 'Library/Technology: Android Studio']">
      <template #title> Driveway </template>

      <template #introduction> 
        An Android application that allows users rent parking spots.
      </template>
    </ExperienceItem>
</template>

<style scoped>
h1{
  color: hsla(160, 100%, 37%, 1);
}
</style>
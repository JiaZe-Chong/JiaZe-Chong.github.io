<script setup>
import ExperienceItem from './components/ExperienceItem.vue'
</script>

<template>
  <header>
    <h1>Jia Ze Chong</h1>
    <p>Junior computer science student</p>
    <p>at Iowa State University</p>
  </header>

  <main>
    <h1 class="pop">Projects:</h1>
    <ExperienceItem :points="['Language: C and C++', 'Library/Technology: nCurses, Makefile']">
      <template #title> Pokemon Game </template>

      <template #takeaway>
        Biggest takeaway: Technical Dept, what seems to be an easy solution for a problem will later
        present itself again in the form of refactoring down the road.
      </template>
    </ExperienceItem>
  </main>
</template>

<style scoped>
.pop {
  color: var(--color-accent);
}
</style>

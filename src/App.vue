<script setup>
import projects from './components/ProjectList.vue'
import myTitle from './components/MyTitle.vue'
import contact from './components/ContactMe.vue'
import work from './components/ExperienceList.vue'
import introduction from './components/MyIntroduction.vue'
</script>

<template>
  <div class="all">
    <myTitle class="item" />
    <introduction class="item" />
    <work class="item" />
    <projects class="item" />
    <contact class="item" />
  </div>
</template>

<style scoped>
.all {
  width: 70vw;
  left: 15vw;
  right: 15vw;
}
.item {
  padding-bottom: 1vw;
}
</style>

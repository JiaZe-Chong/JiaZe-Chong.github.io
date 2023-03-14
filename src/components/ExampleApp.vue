<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import ExperienceItem from './components/ExperienceItem.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div>
  </header>

  <main>
    <TheWelcome />
  </main>

  <ExperienceItem :points="['apple', 'bible', 'cat']">
    <template #title> Title 1 </template>

    <template #takeaway>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nihil distinctio adipisci ex
      inventore, illo aliquam? Impedit, enim dicta. Veritatis, accusamus vero. Reiciendis aperiam, a
      at molestias deserunt dicta nemo corporis.
    </template>
  </ExperienceItem>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>

<script setup>
import projects from './components/ProjectList.vue'
import intro from './components/Introduction.vue'
import contact from './components/ContactMe.vue'
import work from './components/ExperienceList.vue'
</script>

<template>
    <div class = "all">
        <intro />
        <work />
        <projects />
        <contact />
    </div>
    
</template>

<style scoped>
    .all{
        width: 70vw;
        left: 15vw;
        right: 15vw;
    }
</style>
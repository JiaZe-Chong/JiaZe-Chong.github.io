<script setup>
import projects from './components/ProjectList.vue'
import intro from './components/Introduction.vue'
import contact from './components/ContactMe.vue'
</script>

<template>
    <div class = "all">
        <intro />
        <projects />
        <contact />
    </div>
    
</template>

<style scoped>
    .all{
        width: 80vw;
        left: 10vw;
        right: 10vw;
    }
</style>
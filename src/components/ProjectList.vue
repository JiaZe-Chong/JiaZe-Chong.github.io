<script setup>
import ExperienceItem from './ExperienceItem.vue'
</script>

<template>
  <div class="item">
    <h1>Projects:</h1>
    <ExperienceItem>
      <template #title> About Me(this) </template>

      <template #introduction>
        A webpage that introduces myself along with the projects and work experiences I have.
      </template>

      <template #details>
        <p>-Language: <span>Javascript</span></p>
        <p>-Library/Technology: <span>VueJS</span>, <span>Github Pages</span></p>
        <p>-Used <span>conditional rendering</span> to only show details on click.</p>
        <p>-Utilized <span>components</span> to organize code base.</p>
        <p>-Used <span>slots</span> and <span>props</span> to pass data into components.</p>
        <p>
          -Biggest lesson: You can never really learn everything there is to learn about some
          language/framework/library. You just need to learn the fundamental and keep learning while
          you are using it.
        </p>
      </template>
    </ExperienceItem>

    <ExperienceItem>
      <template #title> Pokemon Game </template>

      <template #introduction>
        A Pokemon game with the core gameplay such as random map generation, player movement, random
        occuring events, and combat system implemented.
      </template>

      <template #details>
        <p>-Language: <span>C</span> and <span>C++</span></p>
        <p>-Library/Technology: <span>nCurses</span>, <span>Makefile</span></p>
        <p>-Used <span>nCurses</span> for terminal manipulation and unbuffered input.</p>
        <p>-Developed and used a parser to parse data from a CSV file.</p>
        <p>
          -Utilized <span>object-oriented programming</span> to simplify and streamline the
          development of the game.
        </p>
        <p>-Utilized header files and <span>Makefile</span> to improve code maintainability.</p>
        <p>
          -Biggest lesson: Technical dept, what seems like an easy solution for current complication
          may lead to a much harder problem that needs to be solve, so always plan ahead.
        </p>
      </template>
    </ExperienceItem>

    <ExperienceItem>
      <template #title> Driveway </template>

      <template #introduction>
        An Android application that allows users rent parking spots.
      </template>

      <template #details>
        <p>-Language: <span>Java</span></p>
        <p>
          -Library/Technology: <span>Android Studio</span>, <span>Springboot</span>,
          <span>Git</span>
        </p>
        <p>
          -<span>HTTP requests</span> and <span>WebSockets</span> are used for communication between
          the front-end client and the back-end server.
        </p>
        <p>
          -Implemented <span>CRUD</span> functions using <span>REST API</span> to manipulate data
          stored in the back-end server
        </p>
        <p>-Utilized fragments and activities to make UI more friendly</p>
        <p>
          -Biggest lesson: Plan ahead, as projects get bigger, it is very important to plan ahead as
          even the simplest things such as naming variables can be hard due to namespace pollution
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

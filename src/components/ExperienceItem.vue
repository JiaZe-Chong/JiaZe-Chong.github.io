<script setup>
import { ref } from 'vue'
defineProps({
  points: {
    type: Array,
    required: true
  }
})

const det = ref(false)
</script>

<template>
  <div class="item">
    <div class="title">
      <h1>
        <slot name="title"></slot>
      </h1>
    </div>
    <div class="details">
      <p>
        <slot name="takeaway"></slot>
      </p>
      <button class="btn" @click="det = !det">Details</button>
      <ul v-if="det">
        <li v-for="point in points">
          {{ point }}
        </li>
      </ul>
    </div>
  </div>
</template>

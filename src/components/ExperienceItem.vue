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
      <h3>
        <slot name="title"></slot>
      </h3>
    </div>
    <div class="details">
      <p>
        <slot name="takeaway"></slot>
      </p>
      <button class="btn" @click="det = !det">Details</button>
      <ul v-if="det">
        <li v-for="point in points" v-bind:key="point">
          {{ point }}
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.btn {
  color: #fff;
  background: linear-gradient(315deg, #42d392 25%, #647eff);
  border: none;
  padding: 5px 10px;
  margin: 5px;
  border-radius: 8px;
  cursor: pointer;
}

h1 {
  color: var(--color-heading);
}
p {
  color: var(--color-text);
}
</style>

<script setup>
import { ref } from 'vue'
const det = ref(false)
</script>

<template>
  <div class="item">
    <h3>
      <slot name="title"></slot>
    </h3>
    <p>
      <slot name="introduction"></slot>
    </p>
    <button class="btn" @click="det = !det">Details</button>
    <div v-show="det" class="detail">
      <slot name="details"></slot>
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

.detail {
  width: 90%;
  left: 5%;
  padding-bottom: 30px;
}
</style>

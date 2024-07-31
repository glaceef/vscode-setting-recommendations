<script setup>
import { ref } from 'vue';

const counter = ref(0);

const count = () => {
  counter.value += 1;
}
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
    <div>
      <div @click="count">
        Counter
      </div>
      Count: {{ counter }}
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>

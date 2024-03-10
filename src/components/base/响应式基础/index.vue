<template>
  <div>
    <button @click="increment">
      {{ count }}
    </button>
    <button @click="increments">
      {{ state.counts }}
    </button>
  </div>
</template>

<script setup lang="ts">
import { reactive, ref } from "vue";

const count = ref(0);
const state = reactive({
  counts: 0,
});
const increment = () => {
  count.value++;
};
const increments = () => {
  state.counts++;
};
</script>

<style scoped></style>

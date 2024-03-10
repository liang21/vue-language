<template>
  <div>
    <span>Message:{{ msg }}</span>
    <div :id="dynamicId">
      <button>Click me</button>
    </div>
  </div>
</template>
<script setup lang="ts">
const msg = "Hello World";
const dynamicId = "dynamic-id";
</script>
<style scoped>
button {
  color: red;
}
</style>

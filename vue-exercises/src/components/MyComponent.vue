<script setup lang="ts">
  defineProps<{
    prop: string;
  }>();

  function getCharacteristices(value: string) {
    return `${value.length} characters and the first character is ${value[0]}`;
  }

</script>

<template>
  <h2>This is MyComponent</h2>
  <p>This is a prop: {{ prop }}</p>
  <p>It is a string that has: {{ getCharacteristices(prop) }}.</p>
</template>

<style scoped></style>
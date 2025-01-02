<script setup lang="ts">
const HELLO = import.meta.env.HELLO;
console.log(`HELLO: ${HELLO}`);
console.assert(typeof HELLO === "undefined", "HELLO should be undefined");

const VITE_HELLO = import.meta.env.VITE_HELLO;
console.log(`VITE_HELLO: ${VITE_HELLO}`);
console.assert(
  typeof VITE_HELLO === "string",
  "VITE_HELLO should be a string"
);
</script>

<template>
  <div>
    <h1>SPA-VUE</h1>
    <h1>HELLO:{{ HELLO }} </h1>
    <h1>VITE_HELLO:{{ VITE_HELLO }} </h1>
  </div>
</template>


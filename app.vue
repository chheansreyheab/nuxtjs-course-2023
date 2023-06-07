<template>
  <div>
    Hello World
  </div>
  <button>Increment</button>
  <p>{{ count }}</p>
  <button>Decrement</button>
</template>
<script setup>
import ref from "vue";
const count = ref(0)
</script>

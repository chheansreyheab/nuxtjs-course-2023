<template>
    <button @click="increment">Increment</button>
    <p>{{ count }}</p>
    <button @click="decrement">Decrement</button>
  </template>
  <script setup>
  // export default {
  //   data(){
  //     return{
  //       count: 0,
  //     };
  //   },
  //   methods:{
  //     increment(){
  //       this.count++;
  //     },
  //     decrement(){
  //       this.count--;
  //     },
  //   },
  // };

  
  const count = ref(0);
  function increment(){
    count.value++;
  }
  function decrement(){
    count.value--;
  }
  </script>
  
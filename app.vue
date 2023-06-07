<template>
  <a href="#" @click="view('home')">Home</a>
  <a href="#" @click="view('counter')">Counter</a>
  <HomeWelcome v-if="page == 'home'"/>
  <Counter v-if="page == 'counter'"/>
  <!-- <home-welcome/>
  <button @click="toggle">Toggle</button>
  <component :is="MyComponent" /> -->
  <!-- <Counter/> -->
</template>

<script setup>
const page = ref("home")
function view(name){
  page.value = name
}


// const MyComponent = ref(resolveComponent("Counter"));
// function toggle(){
//   MyComponent.value = resolveComponent("HomeWelcome")
// }
</script>
<template>
    <div>
      <h1>Contador: {{ counter }}</h1>
      <ChildComponent :counter="counter" />
    </div>
  </template>
  
  <script>
  import { ref } from 'vue';
  import ChildComponent from './ChildComponent.vue';
  
  export default {
    components: { ChildComponent },
    setup() {
      const counter = ref(0);
      return { counter };
    },
  };
  </script>
  
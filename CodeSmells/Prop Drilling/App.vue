<template>
    <ParentComponent :user="user" />
  </template>
  
  <script>
  import ParentComponent from './ParentComponent.vue';
  
  export default {
    components: { ParentComponent },
    data() {
      return {
        user: { name: 'João', age: 22 },
      };
    },
  };
  </script>
  
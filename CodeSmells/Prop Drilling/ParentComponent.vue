<template>
    <ChildComponent :user="user" />
  </template>
  
  <script>
  import ChildComponent from './ChildComponent.vue';
  
  export default {
    props: ['user'],
    components: { ChildComponent },
  };
  </script>
  
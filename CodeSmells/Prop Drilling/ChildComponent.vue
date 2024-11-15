<template>
    <TargetComponent :user="user" />
  </template>
  
  <script>
  import TargetComponent from './TargetComponent.vue';
  
  export default {
    props: ['user'],
    components: { TargetComponent },
  };
  </script>
  
<template>
    <div>
      <ChildComponent title="Componente 1" />
      <ChildComponent title="Componente 2" />
      <ChildComponent title="Componente 3" />
    </div>
  </template>
  
  <script>
  import ChildComponent from './FatherComponent.vue';
  
  export default {
    components: { ChildComponent },
  };
  </script>
  
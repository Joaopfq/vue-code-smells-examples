<template>
    <div>
      <p>{{ name }}</p>
      <button @click="updateName">Atualizar Nome</button>
    </div>
  </template>
  
  <script>
  import { reactive } from 'vue';
  
  export default {
    setup() {
      const state = reactive({
        name: 'João',
      });
  
      // Desestruturando a propriedade reativa
      const { name } = state;
  
      function updateName() {
        state.name = 'Paulo';
      }
  
      return {
        name,
        updateName,
      };
    },
  };
  </script>
  
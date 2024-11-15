<template>
    <div>
      <p>{{ message }}</p>
      <button @click="updateMessage">Atualizar Mensagem</button>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        message: 'Mensagem inicial',
      };
    },
    methods: {
      updateMessage() {
        // Alterando diretamente o DOM sem usar a reatividade
        this.message = 'Nova mensagem'; // O Vue não detecta porque o dado não está sendo gerenciado reativamente
        this.$forceUpdate(); // Forçando a renderização para mostrar a mudança
      },
    },
  };
  </script>
  
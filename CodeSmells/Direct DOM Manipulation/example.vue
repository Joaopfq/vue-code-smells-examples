<template>
    <div>
      <p id="message">{{ message }}</p>
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
        const element = document.getElementById('message');
        element.textContent = 'Mensagem atualizada'; // Manipulação direta do DOM
      },
    },
  };
  </script>
  
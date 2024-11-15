<template>
    <div>
      <h1>Bem-vindo!</h1>
      <!-- Renderiza conteúdo fornecido pelo usuário diretamente -->
      <div v-html="userProvidedHtml"></div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        userProvidedHtml: '<img src="invalid.jpg" onerror="alert(\'XSS Attack!\')" />', // Dados inseguros
      };
    },
  };
  </script>
  
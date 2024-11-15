<template>
    <button @click="incrementCounter">Incrementar Contador</button>
  </template>
  
  <script>
  export default {
    props: ['counter'],
    methods: {
      incrementCounter() {
        this.counter++; // Alterando o estado do pai diretamente
      },
    },
  };
  </script>
  
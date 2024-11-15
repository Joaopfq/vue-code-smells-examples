<template>
    <div>
      <h1>{{ title }}</h1>
      <p>{{ description }}</p>
      <button @click="fetchData">Fetch Data</button>
      <ul>
        <li v-for="item in items" :key="item.id">{{ item.name }}</li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        title: 'Título Principal',
        description: 'Descrição do componente',
        items: [],
      };
    },
    methods: {
      fetchData() {
        fetch('https://api.example.com/data')
          .then((response) => response.json())
          .then((data) => {
            this.items = data;
          })
          .catch((error) => console.error(error));
      },
    },
    mounted() {
      console.log('Componente montado!');
    },
  };
  </script>
  
  <style scoped>
  h1 {
    color: blue;
  }
  </style>
  
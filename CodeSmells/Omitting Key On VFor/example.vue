<template>
    <ul>
      <li v-for="item in items">{{ item.name }}</li>
    </ul>
  </template>
  
  <script>
  export default {
    data() {
      return {
        items: [
          { id: 1, name: 'Item A' },
          { id: 2, name: 'Item B' },
          { id: 3, name: 'Item C' },
        ],
      };
    },
  };
  </script>
  
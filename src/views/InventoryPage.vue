<template>
    <div>
      <h1>库存列表</h1>
      <ul>
        <li v-for="item in inventory" :key="item.id">{{ item.name }} - {{ item.quantity }}</li>
      </ul>
    </div>
  </template>
  
  <script>
  import http from '@/utils/http';
  
  export default {
    name: 'InventoryPage',
    data() {
      return {
        inventory: [],
      };
    },
    mounted() {
      http.get('/inventory')
        .then((response) => {
          this.inventory = response.data;
        })
        .catch((error) => {
          console.error(error);
        });
    },
  };
  </script>
  
  <style scoped>
  /* 页面样式 */
  </style>
  
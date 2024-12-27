<template>
    <nav>
      <ul>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/inventory">Inventory</router-link></li>
      </ul>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'AppNavbar',
  };
  </script>
  
  <style scoped>
  nav {
    background-color: #333;
    padding: 10px;
  }
  
  ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
  }
  
  li {
    margin-right: 20px;
  }
  
  a {
    color: white;
    text-decoration: none;
  }
  </style>
  
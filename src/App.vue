<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <div>
    <AppNavbar />
    <router-view />
  </div>
</template>

<script>
import AppNavbar from './components/AppNavbar.vue';  // 导入修改后的组件

export default {
  name: 'App',
  components: {
    AppNavbar,  // 使用修改后的组件名
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

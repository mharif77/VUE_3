<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  
  <NewYearVue/>
  <FruitItemVue/>

</template>

<script>
import FruitItemVue from './components/FruitItem.vue'


import NewYearVue from './components/NewYear.vue'





export default {
  name: 'App',
  components: {
    NewYearVue,FruitItemVue
  }
}
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

<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
    <div class="wrapper">lifecycle
      form
      

      <nav>
        <RouterLink to="/">Home</RouterLink> |
        <RouterLink to="/food">Food Item</RouterLink> |
        <RouterLink to="/fruit">Fruit Item</RouterLink> |
        <RouterLink to="/todo">Todo list</RouterLink> |
         <RouterLink to="/ref">Reference Hook</RouterLink> |
         <RouterLink to="/lifecycle">lifecycle Hooks</RouterLink> |
         <RouterLink to="/form">Form inputs</RouterLink> |
         <RouterLink to="/flowers">flowers</RouterLink> |
         <RouterLink to="/flowerlist">flowerlist</RouterLink> |


      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style>

</style>

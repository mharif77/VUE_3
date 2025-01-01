<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HeaderViewVue from './components/HeaderView.vue'


</script>

<template>
  <HeaderViewVue/>

  <RouterView />
  <div class="jumbotron text-center" style="margin-bottom:0">
  <p>Footer</p>
</div>
</template>



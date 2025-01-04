<template>
   <!-- <div v-on:click="countClicks">
    <h2>{{ name }}</h2>  
    <p>{{ message }}</p>
    <p id="green">You have clicked me {{ clicks }} times.</p>
    
  </div> -->


  <div>
      <h1>  {{foodName}}</h1>
      <p>{{foodDesc}}</p>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                 name: 'Apples',
                message: 'I like apples',
                clicks: 0
            }
        },
         methods: {
    countClicks() {
      this.clicks++;
        }
    },
    props: [
        'foodName',
        'foodDesc'
    ]
}
</script>

<style>

</style>
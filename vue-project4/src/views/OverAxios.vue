<template>
    <div>
        <button @click="callData">click here this </button>
<h1 v-if="mydata"><pre>{{mydata}}</pre></h1>
    </div>
    
</template>

<script setup>
import axios from 'axios';
</script>

<script>

    export default {
        data() {
            return {
                mydata:null
            }
        },
        methods:{
          async  callData(){
               
             let response = await  axios.get('https://random-data-api.com/api/v2/users');
           this.mydata = response;
            }
        },
    }
</script>






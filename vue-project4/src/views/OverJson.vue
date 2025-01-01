<template>
    <div>
        <button @click="callData">click </button>
<h1 v-if="mydata"><pre>{{mydata}}</pre></h1>
    </div>
    
</template>

<script>
    export default {
        data() {
            return {
                mydata:null
            }
        },
        methods:{
          async  callData(){
               
             let response = await  fetch('src/assets/myData.json');
           this.mydata = await response.json();
            }
        },
    }
</script>


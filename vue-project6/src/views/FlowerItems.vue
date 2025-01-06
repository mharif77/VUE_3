<template>
    <div>
<ul>
    <li v-for="x in flowers" :key="x">{{ x.name }}</li>
</ul>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                flowers:[
                  { name:'Flower1', url:'a1.jpg'},
                  { name:'Flower2', url:'a2.jpg'},
                  { name:'Flower3', url:'a3.jpg'},
                  { name:'Flower4', url:'a4.jpg'},
                  { name:'Flower5', url:'a5.jpg'}
                ]
            }
        },
        provide(){
            return{
                flowers:this.flowers
            }
        }
    }
</script>

<style scoped>

</style>
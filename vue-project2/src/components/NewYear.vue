<template>
    <div>
<h1 v-bind:class="ClassName">Happ new Year 2025</h1>
<img v-bind:src="url" alt="" width="400px" height="200px">
<hr>
<p v-if="productsInStock">
  in stock
</p>

<p v-else>
  not in stock
</p>
    </div>
</template>

<script>
    export default {
        
         data() {
            return {
               ClassName: "head",
               url: require("@/newyear.jpg"),
               productsInStock:true

            }
        },
        
    }
</script>

<style>
.head{
    color: green;
    font-size: 50px;
    text-align: center;
    background-color: cornflowerblue;

}

</style>
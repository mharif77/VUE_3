

<template>
  <h1>Welcome Here</h1>
  <h3>Food Item global component coming from Main.js</h3>
   <food-item food-name="Moghlai" food-desc="bhajapora"/>
    <food-item food-name="rice" food-desc="I like it"/>
     <food-item food-name="puri" food-desc="I hate this food"/>
   
    <food-item food-name="pizza" food-desc="nothig comment"/>
    <hr>
 <product-item product-name="pant" product-desc="black pant"  v-bind:is-favourite="true" />
 <product-item product-name="shirt" product-desc="white shirt"  v-bind:is-favourite="false" />
</template>


<style>
  #app > div {
        border: dashed black 2px;
        display: inline-block;
        margin: 20px;
        padding: 20px;
        background-color: cornflowerblue;
    }

    #app > div:hover {
  cursor: pointer;
}
</style>  

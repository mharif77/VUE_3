<template>
    <div class="box">
<h3>{{productName}}</h3>
<img src="/src/assets/1.jpg" width="50" alt="" v-show="isFavourite">
<p>{{productdesc}}</p>
    </div>
</template>

<script>
    export default {
          props: ['productName','productDesc','isFavourite']
    }
</script>

<style>
.box{
    height: 100px;
    width: 80px;
    border: 1px solid goldenrod;
    float: left;
}
img{
    float: right;
}
</style>
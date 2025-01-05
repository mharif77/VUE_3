<template>
    <div>
        <button @click="showData">click here</button>
<h1 ref="h1content"></h1>
    </div>
    <div>
        <hr>
        <p ref="msg">Today is first sunday of current year</p>
        <button @click="copyPaste">Click here</button>
        <h1 ref="msgShow">.......</h1>
    </div>

    <form action="">
        <input type="text" name="fullname" ref="fullname" @input="inputShow">
        <h1 ref="nameShow"></h1>
    </form>
</template>

<script>
    export default {
        methods: {
            showData(){
              this.$refs.h1content.innerHTML
               =  "Hello world";
            },

            copyPaste(){
                this.$refs.msgShow.innerHTML
               = this.$refs.msg.innerHTML
            },

            inputShow(){
                this.$refs.nameShow.innerHTML
               = this.$refs.fullname.value;
            }
        },
    }
</script>

<style scoped>

</style>
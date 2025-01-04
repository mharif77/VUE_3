<template>
    <div>
        <h1>Todo List</h1>
        <ul>
            <todo-item v-for="x in contents" :key="x" :todo-name="x" />
        </ul>
        <input type="text" v-model="newContent" v-on:keydown.enter="addContents">
        <button @click="addContents">add</button>
    </div>
</template>

<script>

    export default {
        data() {
            return {
                contents:[
                    'laptop',
                    'mouse',
                    'keyboard'
                ],
                newContent: ''
            }
        },
        methods: {
        addContents(){
            this.contents.push(this.newContent)
             this.newContent = ''
        }
    }
    }
</script>


<style>

</style>
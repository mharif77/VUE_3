<template>
    <div>
<ul>
    <li v-for="x in fruits" :key="x">
    {{x}}</li>
</ul>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                fruits: [
                    'apple',
                    'mango',
                    'grape'
                ]
            }
        },
    }
</script>

<style>

</style>
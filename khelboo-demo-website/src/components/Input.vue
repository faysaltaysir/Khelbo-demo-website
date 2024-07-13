<template>
    <input type="text" :placeholder="placeHolder" v-model="inputValue">
</template>
<style scoped>
    input{
        width: 10rem;
        border-radius: 40px;
        padding: 5px 0px 5px 10px;
        font-style: italic;
        font-size: 1.1rem;
        border: 1px solid black;
    }
</style>
<script>
    export default{
        props:['placeHolder'],
        data(){
            return{
                inputValue:this.placeHolder,
            }
        }
    }
</script>
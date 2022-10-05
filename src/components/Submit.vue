<script setup>
  import { NDivider } from 'naive-ui'
</script>

<template>
    <button id="submit-button" class="button">Submit</button>
</template>

<style scoped>
.button{
    width: 60px;
    height: 30px;

    font-size:10px;
    font-weight: 600;
    font-family: Arial, Helvetica, sans-serif;

    box-sizing: border-box;
    border: 2px solid balck;
    margin: 0;

    background-color: rgb(14, 201, 129);   
}
.button:hover{
    cursor: pointer;
    background-color: rgb(43, 234, 160);
}
.button:active{
    background-color: rgb(14, 144, 94);
}
.button:disabled{
    background-color: rgb(14, 144, 94);
    cursor: not-allowed;
}   
</style>
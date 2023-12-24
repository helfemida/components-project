<template>
    <div class="container" id="container">
        <div class="element" :style="{ backgroundColor: backgroundColor, height: height, width:width }"></div>
        <label for="element"> {{elementName}}</label>
    </div>
</template>

<script>
    export default{
        el: '#container',
        props:{
            elementName: String,
            backgroundColor: String,
            height: String,
            width: String
        }
    }
</script>

<style>
    .container{
        width: 100%;
        height: 100%;
        align-items: center;
        display: flex;
        flex-direction: column;
        font-size: 70%;
        color: rgba(162,154,176,255);
        font-weight: 600;
    }
    .element{
        background-color: aqua;
        width: 70%;
        height: 100%;
        margin-bottom: 20%;
    }
    .label{
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        
        
    }
    
    
</style>


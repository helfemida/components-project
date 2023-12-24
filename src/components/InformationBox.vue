<template>
    <div class="box" id="box">
        <p class="infoHeader"> {{infoHeader}}</p>
        <p class="infoDescription">{{infoDescription}}</p>
    </div>
</template>

<script>
    export default{
        name: 'InformationBox',
        el: '#box',
        props:{
            infoHeader: String,
            infoDescription: String
        }
    }
</script>

<style>
    .box{
        display: flex;
        flex-direction: column;
        width: 100%;
        height: 30%;
    }
    .infoHeader{
        font-weight: 600;
        font-size: 130%;
        padding-bottom: 5%;
    }
    .infoDescription{
        font-size: 100%;
        font-weight: 200;
        color: #a49db2;
    }
</style>
<template>
    <LatestTransactions></LatestTransactions>
</template>
<script>
import LatestTransactions from './components/LatestTransactions.vue';
    export default{
        components:{
            LatestTransactions
        }
    }
</script>
  
<style>
    *{
        box-sizing: border-box;
        padding: 0;
        margin:0;
    }
    body{
        color: navy;
        font-family: Verdana, Geneva, Tahoma, sans-serif;
    }
    .main{
        width: 600px;
        height: 900px;
        margin: 0% 2%;
    }
</style>
  
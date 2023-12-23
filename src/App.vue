<template>
    <Header></Header>
</template>
  
<script>
    import Header from './components/Header.vue';
  
    export default {
        name: 'App',
        components: {
        Header
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
</style>
  
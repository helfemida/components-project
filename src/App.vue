<template>
    <Header></Header>
    <section class="main">
        <MenuBar></MenuBar>
        <div class="banking-section">
            <div class="heading">
                <InfoBox infoHeader="Hello" infoDescription="hello"></InfoBox>
            </div>
        </div>
    </section>
</template>
  
<script>
    import Header from './components/Header.vue';
    import MenuBar from './components/MenuBar.vue';
    import InfoBox from './components/InfoBox.vue';

    export default {
        name: 'App',
        components: {
        Header,
        MenuBar,
        InfoBox
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
        margin: 0% 2%;
    }
</style>
  
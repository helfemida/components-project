<template>
    <div class="container">
        <h2>Recent Activity</h2>
        <div class="el">
            <img :src="require('@/assets/income.png')" alt="">
            <p>+$2000</p>
        </div>
        <div class="el">
            <img :src="require('@/assets/income.png')" alt="">
            <InformationBox infoHeader="Subscription" infoDescription="2 March 2021, 13:45"></InformationBox>
            <p>-$120</p>
        </div>
    </div>
</template>

<script>
import InformationBox from './InformationBox.vue';
export default{
    components:{
        InformationBox
    }
}
</script>

<style scoped>

.container{
    width: 300px;
    height: 250px;

    display: flex;
    flex-direction: column;
}
.el{
    display: flex;
    width: 70%;
    height: 100%;
}

.el img{
    width: 30px;
    height: 30px;
}

</style>
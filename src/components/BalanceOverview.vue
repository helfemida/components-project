<template>
   <div class="top-container">
        <div class="text-info">
            <InformationBox infoHeader="Your Balance" infoDescription="June 1, 2020, 08:22 AM"></InformationBox>
            <div class="amount">
                <InfoboxReverse infoHeader="This Month" infoDescription="$23,741.00"></InfoboxReverse>
                <div class="percent-info">
                    <img :src="require('@/assets/up-arrow.png')" alt="">
                    <p>+15%</p>
                </div>
            </div>
        </div>
        <WeeklyGraph></WeeklyGraph>
   </div>

   <div class="bottom-container">
    <div class="el-1">
        <img :src="require('@/assets/income.png')" alt="">
        <InfoboxReverse infoHeader="Income" infoDescription="$23,741.00"></InfoboxReverse>
    </div>
    <div class="el-1">
        <img :src="require('@/assets/income.png')" alt="">
        <InfoboxReverse infoHeader="Outcome" infoDescription="$23,741.00"></InfoboxReverse>
    </div>
   </div>
</template>

<script>
    import InformationBox from './InformationBox.vue';
    import InfoboxReverse from './InfoboxReverse.vue';
    import WeeklyGraph from './WeeklyGraph.vue';

    export default{
        components:{
            InfoboxReverse,
            WeeklyGraph,
            InformationBox
        }
    }
</script>

<style>
    .text-info{
        display: flex;
        flex-direction: column;
        margin: 2% 0;
        
    }
    .top-container{
        display: flex;
        flex-direction: row;
        margin:0 2% ;
        justify-content: space-between;
        width: 60%;
        height: 40%;
    }
    .percent-info{
        width: 50px;
        height: 30px;
        display: flex;
        flex-direction: row;
        color: #4cbc9a;
        font-weight: bolder;
        align-items: center;
        font-size: 15px;
        position: relative;
        padding-top: 65px;
    }
    .amount{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        height: 40%;
        padding-top: 40px;
    }
    .percent-info img{
        width: 30px;
        height: 30px;
        padding: 5px;
    }
    .bottom-container {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        width: 650px;
        padding-left: 30px;
        padding-top: 20px;
    }
    .el-1{
        display: flex;
        width: 250px;
        height: 130px;
        display: flex;
        flex-direction: row;
        align-content: center;
        position: relative;
    }

    .el-1 img{
        widows: 70px;
        height: 70px;
        padding-right: 20px;
    }

    

</style>


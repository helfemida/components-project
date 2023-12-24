<template>
    
    <div class="userinfo-container">
        <div class="user">
            <img :src="require(`@/assets/${imageName}`)" class="userImg" alt="">
            <p>{{nameSurname}}</p>
        </div>

        <p class="amount">{{amount}}</p>
        <p class="date">{{date}}</p>
        
        <div class="transaction-buttons">
            <img :src="require('@/assets/print.png')" alt="">
            <img :src="require('@/assets/more.png')" alt="">
        </div>
        
    </div>
</template>

<script>
    export default{
        
        props:{
            imageName: String,
            nameSurname: String, 
            amount: String,
            date: String
        }
    }
</script>

<style>
    .userinfo-container{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        color: #324160;
        font-size: 15px;
        padding: 20px;
        width: 600px;
    }
    .user, .amount{
        display: flex;
        width: 1/4;
        align-items: center;
        font-weight: 600;
        height: 50px;
    }
    
    .date{
        color: #999aae;
        font-size: 13px;
        width: 1/4;
        text-align: center;
        height: 50px;
        text-align: center;
    }
    .userImg{
        width: 40px;
        height: 40px;
        border: 0px solid transparent;
        border-radius: 13px;
        margin-right: 20px;
    }
    
    .transaction-buttons{
        width: 1/4;
        
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        height: 50px;
        
    }
    .transaction-buttons img{
        width: 40px;
        height: 25px;
        padding-right: 15px;

    }</style>

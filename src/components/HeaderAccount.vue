<template scoped>
    <div class="account-container">
        <div class="user">
            <p class="name">Sth Sth</p>
            <p class="tag">Admin</p>
        </div>
        <img :src="require('@/assets/user.png')" alt="">
    </div>
</template>

<style scoped>
    .account-container{
        width: 200px;
        height: 50px;
        display: flex;
        align-items: center;
        
    }
    .name{
        font-weight: 600;
        padding-bottom: 5px;
        font-size: 10px;
    }
    .tag{
        font-weight: 200;
        font-size: 12px;
    }
    .account-container img{
        width: 60px;
        height: 45px;
        padding-left: 15px;
    }
</style>

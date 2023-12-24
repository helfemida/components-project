<template>
    <div class="container">
        <div class="heading">
            <p class="container-header">Latest Transactions</p>
            <div class="buttons">
                <SimpleButton title="This Month" imageName="down.png"></SimpleButton>
                <img class="more-button" src="../assets/more.png" alt="">
            </div>
        </div>
        <UsersHistory></UsersHistory>

        <div class="footer-container">
            <p>Showing 1-5 from 100</p>
            <div class="footer-buttons">
                <img class="arrow-button" src="../assets/left-arrow.png" alt="">
                <div class="number-button">1</div>
                <div class="number-button-2">2</div>
                <div class="number-button">3</div>
                <img class="arrow-button" src="../assets/right-arrow.png" alt="">
            </div>
        </div>

    </div>
</template>

<script>
import SimpleButton from './SimpleButton.vue';
import UsersHistory from './UsersHistory.vue';
export default{
    components:{
        SimpleButton,
        UsersHistory
    }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&family=Open+Sans:ital,wght@0,400;0,500;0,700;1,600&display=swap');

.container{
    display: flex;
    flex-direction: column;

    width: 80%;
    height: 70%;
    align-items: center;
    justify-content: center;

    border: 1px solid black;   
}

.heading{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;

    width: 100%;
    height: 20%;
    padding: 0 20px ;
    
}
.buttons{
    width: 30%;
    height: 100%;

    display: flex;
    flex-direction: row;
    align-items: center;

}

.more-button{
    width: 25px;
    height: 25px;
    margin: 12px;
}

.container-header{
    font-family: 'Montserrat', sans-serif;
    font-size: 25px;
    font-weight: bold;
}
.number-button{
    background-color: #fbeeea;
    color: #ef6d4d;
    width: 50px;
    height: 50px;
    text-align: center;
    margin: 10px;
    font-size: 20px;
}
.number-button-2{
    display: flex;
    background-color:  #ef6d4d;
    color: #fbeeea ;
    width: 50px;
    height: 50px;
    text-align: center;
    justify-content: center;
    margin: 10px;
    font-size: 20px;
}
.footer-container{
    display: flex;
    width: 100%;
    height: 20%;

    justify-content: space-between;
    align-items: center;
    text-align: center;
}
.footer-buttons{
    display: flex;
    flex-direction: row;
}
.arrow-button{
    width: 50px;
    height: 50px;
}

</style>
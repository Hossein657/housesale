<template>
<div class="card_container">
    <div class="card" v-for="content in contents" :key="content.id">
        <img :src="content.img" :alt="content.title">
        <div class="bottom">
        <ion-icon name="chevron-forward-circle"></ion-icon>
        <router-link to="/">{{content.title}}</router-link>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: "Cards",
    data(){
        return {
            contents: [
                {title: "Same great quality. New lower prices.", img: require("../assets/cards/card1.png"), id:"1"},
                {title: "Everyday Essentials, High quality affordable ", img: require("../assets/cards/card2.png"), id:"2"},
                {title: "Join the makeover journey ", img: require("../assets/cards/card3.png"), id:"3"},
            ],
        }
    }

}
</script>

<style scoped>
.card_container{
    display: flex;
    
    justify-content: space-between;
}
.bottom{
    min-height: 100px;
    box-shadow: 0px 4px 59px -14px rgba(171, 124, 0, 0.4);
    display: flex;
    align-items: center;
    transition: all .3s;
}
ion-icon{
    font-size:40px;
    color: #FFC839;
    margin: 0 10px;
    transition: all .3s;
    filter: drop-shadow( 1px 4px 4px rgba(0, 0, 0, 0.1));
}
.card{
    transition: all .3s;
}
.card:hover{
    transform: scale(1.01) translateY(-5px);
}
.card:hover .bottom{
    box-shadow: 0px 4px 59px -14px rgba(171, 124, 0, 1);
    background-color: #FFC839;
}
.card:hover ion-icon{
    color: #fff;
}

</style>
<script >
export default{
  data(){
    return{
        cards : [
            { 
                img : "buy-comics-digital-comics.png",
                text : "Digital Comics"
            },
            { 
                img : "buy-comics-merchandise.png",
                text : "DC Merchandise"
            },
            { 
                img : "buy-comics-shop-locator.png",
                text : "Subscription"
            },
            { 
                img : "buy-comics-subscriptions.png",
                text : "Comic Shop Locator"
            },
            { 
                img : "buy-dc-power-visa.svg",
                text : "DC Power Visa"
            }
        ]
    }
  }
}

</script>

<template>
<div class="blueSection">
    <div class="container">
        <div class="card" v-for="(card,index) in cards" :key="index">
            <img :src="card.img" :alt="card.text">
            <span>{{card.text.toUpperCase()}}</span>
        </div>
    </div>
</div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
.blueSection{
    background: $bg-blue;
    height: 20vh;
    display: flex;
    justify-content: space-around;
    z-index: 2;
    position: relative;
    .container{
        max-width: 1300px;
        margin: 0 auto;
        display: flex;
        gap: 70px;

     }
     .card{
        display: flex;
        align-items: center;
        color: white;
        font-size: $font-size-primary;
        gap: 20px;
        img{
            width: 50px;
        }
        span{
            white-space: nowrap;
        }
     }
}

</style>

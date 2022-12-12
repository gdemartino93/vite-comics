<script >
export default{
  data(){
    return{

    }
  }
}

</script>

<template>
<section class="social">
    <div class="container">

        <a href="" class="btn">SIGN-UP NOW!</a>
        <div class="contact"> 
            <span>FOLLOW US</span>
            <img src="../../public/footer-facebook.png" alt="">
            <img src="../../public/footer-twitter.png" alt="">
            <img src="../../public/footer-youtube.png" alt="">
            <img src="../../public/footer-pinterest.png" alt="">
            <img src="../../public/footer-periscope.png" alt="">
        
        </div>
    </div>
</section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
.social{
    background: #333333;


    .container{
        max-width: 1300px;
        margin:  0 auto;
        display: flex;
        align-items: center;
        height: 15vh;
        justify-content: space-between;
        .btn{
            padding: 10px 10px;
            border: 2px solid $bg-blue;
            color: white;
        }
        .contact{
            color: $bg-blue;
            font-weight: bold;
            display: flex;
            gap:20px;
            align-items: center;
        }

    }
}
</style>

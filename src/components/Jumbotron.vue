<script >
export default{
  data(){
    return{

    }
  }
}

</script>

<template>
<div class="jumbotron">
    <img src="https://d2duuy9yo5pldo.cloudfront.net/dashboard-resources/ubisoft-mobile/ff83d81a-db24-454b-aa58-bd2c5a80bd3b.png" alt="">
    <div class="current">CURRENT SERIES</div>
</div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
.jumbotron{
    display: flex;
    height: 200px;
    position: relative;
    img{
        width: 100%;
    }
    .current{
        padding: 10px 10px;
        background: $bg-blue;
        position: absolute;
        bottom: -11%;
        left: 7%;
        color: white;
        font-weight: bold;
        font-size: 20px;
    }
}

</style>

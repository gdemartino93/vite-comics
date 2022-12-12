<script >
export default{
  data(){
    return{
        msg : "work in progress"
    }
  }
}

</script>

<template>
    <main>
        <div class="container">
            {{msg}}
        </div>
   
    </main>

</template>

<style lang="scss" scoped>

main{
    background: black;
    color: white;
    font-weight: bold;
    font-size: 30px;
    .container{
        max-width: 1300px;
        margin: 0 auto;
        display: flex;
        align-items: center;
        height: 15vh;
    }
}   

</style>

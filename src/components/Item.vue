<script >
export default{
  props: {
    itemVue : Object
  },
  data(){
    return{

    }
  }
}

</script>

<template>
    <div class="item">
                <div class="img">
                  <img :src="itemVue.thumb" alt="">
                </div>
                <div class="text">{{itemVue.series}}</div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
.item{
            width: 200px;
            height: 200px;
            border: 1px solid red;
            .img{
                background:pink;
                height: 80%;
            }
            .text{
                background: yellow;
                height: 20%;
                color: black;
            }
        }
</style>

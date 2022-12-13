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
                <div class="text">{{itemVue.series.toUpperCase()}}</div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
.item{
            width: 200px;
            height: 200px;
            margin: 10px;
            cursor: pointer;
            &:hover{
              animation: flash; /* referring directly to the animation's @keyframe declaration */
              animation-duration: 2s; /* don't forget to set a duration! */
            }
            .img{
                height: 80%;
                img{
                  width: 100%;
                  height: 100%;
                }
            }
            .text{
                height: 20%;
                font-size: 15px;
                margin-top: 20px;
            }
        }
</style>

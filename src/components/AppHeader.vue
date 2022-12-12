<script >
export default{
  data(){
    return{
      links : [
        {
          text : "Characters",
          url : "#",
          current : false
        },
        {
          text : "Comics",
          url : "#",
          current : false
        },
        {
          text : "Movies",
          url : "#",
          current : false
        },
        {
          text : "TV",
          url : "#",
          current : false
        },
        {
          text : "Games",
          url : "#",
          current : false
        },
        {
          text : "Collectibles",
          url : "#",
          current : true
        },
        {
          text : "Videos",
          url : "#",
          current : false
        },
        {
          text : "Fans",
          url : "#",
          current : false
        },
        {
          text : "News",
          url : "#",
          current : false
        },
        {
          text : "Shop",
          url : "#",
          current : false
        },

      ]
    }
  }
}

</script>

<template>
  <header>
    <a href="">
      <img src="../../public/dc-logo.png" alt="">
    </a>
    <ul>
      <li v-for="(link, index) in links" :key="index">
        <a :href="link.url" :class="{active: link.current}">
          {{(link.text).toUpperCase()}}
        </a>
      </li>
    </ul>
  </header>
</template>

<style lang="scss" scoped>

header{
  max-width: 1300px;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 0 auto;

 ul{
  display: flex;
  list-style: none;
  gap: 20px;
    a{
    text-decoration: none;
    color: black;
    font-weight: bold;
    }
 }
}

</style>

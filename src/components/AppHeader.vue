<script >
export default{
  props:{
    links : Array
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
@use '../styles/partials/variables' as *;
header{
  padding: 15px 0;
  max-width: 1300px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 0 auto;
  height: 15vh;
 ul{
  display: flex;
  list-style: none;
  gap: 20px;

  // problema con hover
  height: 137%;
  li{
      display: flex;
      align-items: center;
      &:hover{
        border-bottom: 5px solid $bg-blue;
      }
    }
    a{
    text-decoration: none;
    color: black;
    font-weight: bold;

    &:hover{
      color: $bg-blue;
    }
    }
 }
}

</style>

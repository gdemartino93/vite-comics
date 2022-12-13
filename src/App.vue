<script >
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import BluSection from './components/BluSection.vue'
import FooterLink from './components/FooterLink.vue'
import Social from './components/Social.vue'
export default{
  name : "App",
  components :{ AppHeader, AppMain, BluSection, FooterLink, Social} ,
  data(){
    return{
      menu : [
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
  <AppHeader :links="menu" />
  <AppMain />
  <BluSection />
  <FooterLink :links="menu" />
  <Social />
</template>

<style lang="scss" >
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;



</style>

<script >
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import BluSection from './components/BluSection.vue'
import FooterLink from './components/FooterLink.vue'
import Social from './components/Social.vue'
export default{
  name : "App",
  components :{ AppHeader, AppMain, BluSection, FooterLink, Social} 
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <BluSection />
  <FooterLink />
  <Social />
</template>

<style lang="scss" >
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;



</style>

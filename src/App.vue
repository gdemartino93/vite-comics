<script >
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import BluSection from './components/BluSection.vue'
import FooterLink from './components/FooterLink.vue'
export default{
  name : "App",
  components :{ AppHeader, AppMain, BluSection, FooterLink} 
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <BluSection />
  <FooterLink />
</template>

<style lang="scss" >
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;



</style>

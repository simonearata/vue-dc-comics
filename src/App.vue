<template>
  <div id="app">

    <header-comp /> 

    <main-comp />

    <marketing-comp />

    <footer-comp />

  </div>
</template>

<script>
import FooterComp from './components/FooterComp.vue'
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import MarketingComp from './components/MarketingComp.vue'


export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    MarketingComp,
    FooterComp

    
  }
}
</script>

<style lang="scss">

@import './assets/style/App/general.scss';
@import './assets/style/App/utilities.scss';

 
</style>

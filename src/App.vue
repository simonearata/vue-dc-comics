<template>
  <div id="app">

    <header-comp /> 

    <main-comp />

  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'


export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp
    
  }
}
</script>

<style lang="scss">

  *{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  }

  body{
    min-width: 1500px;
  }

  ul{
    list-style: none;
  }

  .container{
    width: 75%;
    margin: auto;
  }

</style>

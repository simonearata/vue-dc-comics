<template>

  <main>
    <div class="fumetti">
      <div class="container">
        <figure-main 
          v-for="(fumetti, index) in figure" 
          :key="index"
          :figures="fumetti"
        />
        <button>LOAD MORE</button>
      </div>
    </div>
  </main>
  
</template>

<script>
import figure from "@/assets/data/dc-comics.js";
import FigureMain from './FigureMain.vue';

export default {
  name: 'MainComp',
  components:{
    FigureMain
  },
  data(){
    return{
      figure
    }
  },
  mounted(){
    console.log(figure);
  }
}
</script>

<style lang="scss" scoped>

  .fumetti{
    background-color: #1c1c1c;
    .container{
      display: flex;
      flex-basis: calc(100% / 7);
      flex-wrap: wrap;
    }
  }




</style>
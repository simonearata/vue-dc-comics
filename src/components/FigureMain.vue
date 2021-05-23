<template>
  <div class="immagini">
    <div class="container-img">
      <img :src="figures.thumb" :alt="figures.series">
    </div>
    <h3>{{ figures.series }}</h3>
  </div>
</template>

<script>
export default {
  name: 'FigureMain',
  props:{
    figures: Object
  }
}
</script>

<style lang="scss" scoped>
  .immagini{
    width: 160px;
    margin-left: 24px;
    margin-top: 40px;
    .container-img{
      width: 160px;
      height: 160px;
      overflow: hidden;
    }
    h3{
      font-size: 13px;
      color: white;
      margin-top: 20px;
      text-transform: uppercase;
    }
  }
</style>
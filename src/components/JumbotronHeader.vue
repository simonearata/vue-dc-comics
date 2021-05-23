<template>
  <div class="cont_jumb">
    <div class="contenitore-text">
      <p>CURRENT SERIES</p> 
    </div>
  </div>
</template>

<script>
export default {
  name: 'JumbotronHeader'
}
</script>

<style lang="scss" scoped>
  .cont_jumb{
    height: 300px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    position: relative;
    .contenitore-text{
      display: inline-block;
      width: 206px;
      height: 33px;
      position: absolute;
      bottom: -15px;
      left: 9px;
      color: white;
      font-size: 19px;
      text-align: center;
      line-height: 33px;
      background-color: #0282f9;
    }
  }
</style>
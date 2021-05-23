<template>

  <div class="informazioni">
    <div class="container">
      <ul>
        <li
          v-for="(info, index) in infos" :key="index"
        >
          <img :src=" info.img " alt="">
          <a href="">{{ info.text }}</a>
        </li>
      </ul>
    </div>
  </div>

</template>

<script>
export default {
  name: 'MarketingComp',
  data(){
    return{
      infos:[
        {
          text:'Digital comics',
          url:'/',
          img:require('../assets/img/buy-comics-digital-comics.png'),
        },
        {
          text:'dc merchandise',
          url:'/',
          img:require('../assets/img/buy-comics-merchandise.png')
        },
        {
          text:'subscription',
          url:'/',
          img:require('../assets/img/buy-comics-subscriptions.png')
        },
        {
          text:'comic shop locator',
          url:'/',
          img:require('../assets/img/buy-comics-shop-locator.png')
        },
        {
          text:'dc power visa',
          url:'/',
          img:require('../assets/img/buy-dc-power-visa.png')
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

 @import '../assets/style/MarketingComp/style.scss';

</style>
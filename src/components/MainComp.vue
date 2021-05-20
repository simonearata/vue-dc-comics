<template>

  <main>
   
    <div class="fumetti">
      <div class="container">

      </div>
    </div>

    <div class="informazioni">
      <div class="container">
        <ul>
          <li
            v-for="(info, index) in infos" :key="index"
          >
            <img :src="'info.img'" alt="">
            <a href="">{{ info.text }}</a>
          </li>
        </ul>
      </div>
    </div>

    
  </main>
  
</template>

<script>
export default {
  name: 'MainComp',
   data(){
    return{
      infos:[
        {
          text:'Characters',
          url:'/',
          img: '../assets/img/buy-comics-digital-comics.png'
        },
        {
          text:'Comics',
          url:'/',
          img:'../assets/img/buy-comics-digital-comics.png'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

  .fumetti{
    background-color: #1c1c1c;
  }

  .informazioni{
    background-color: #0282f9;
    ul{
      display: flex;
      justify-content: space-around;
      align-items: center;
      li{
        display: flex;
        align-items: center;
        img{
          width: 50px;
        }
      }
      
    }
  }

  .container{
    height: 200px;
  }



</style>
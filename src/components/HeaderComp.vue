<template>
  <header>

    <div class="container">
      <a href="/">
        <img src="../assets/img/dc-logo.png" alt="">
      </a>

      <nav>
        <ul>
          <li 
            v-for="(link, index) in links" :key="index"
          >
            <a href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HaederComp',
  data(){
    return{
      links:[
        {
          text:'Characters',
          url:'/',
          flag:'false'
        },
        {
          text:'Comics',
          url:'/',
          flag:'true'
        },
        {
          text:'Movies',
          url:'/',
          flag:'false'
        },
        {
          text:'Tv',
          url:'/',
          flag:'false'
        },
        {
          text:'Collectibles',
          url:'/',
          flag:'false'
        },
        {
          text:'Videos',
          url:'/',
          flag:'false'
        },
        {
          text:'Fans',
          url:'/',
          flag:'false'
        },
        {
          text:'News',
          url:'/',
          flag:'false'
        },
        {
          text:'Shop',
          url:'/',
          flag:'false'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>


  .container{
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  img{
    width: 75px;
  }

  nav{
    ul{
      display: flex;
      justify-content: flex-end;
      li{
        margin: 0 20px;
      }
      a{
        text-decoration: none;
        text-transform: uppercase;
        font-size: 14px;
        font-weight: bold;
        color: #4f5559;
        &:hover,
        &.active{
          border-bottom: 4px solid #0282f9;
          color: #0282f9;
        }

      }
    }
  }

</style>
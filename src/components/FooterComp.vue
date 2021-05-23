<template>

  <footer>
    <div class="container">

      <!-- colonna sinistra -->
      <div class="col-left">

        <!-- prima colonna -->
        <div class="prima-colonna">
          <h3>dc comics</h3>
          <ul>
            <li
              v-for="(dccomic, index) in dccomics" :key="index"
            >
              <a href="dccomic.url">{{ dccomic.text }}</a>
            </li>
          </ul>

          <h3>shop</h3>
          <ul>
            <li
              v-for="(shop, index) in shops" :key="index"
            >
              <a href="shop.url">{{ shop.text }}</a>
            </li>
          </ul>
        </div>

        <div class="colonna-centrale">
          <h3>dc</h3>
          <ul>
            <li
              v-for="(dc, index) in dcs" :key="index"
            >
              <a href="dc.url">{{ dc.text }}</a>
            </li>
          </ul>
        </div>

        <div class="colonna-destra">
          <h3>sites</h3>
          <ul>
            <li
              v-for="(site, index) in sites" :key="index"
            >
              <a href="site.url">{{site.text}}</a>
            </li>
          </ul>
        </div>
      </div>

      <!-- colonna destra -->
      <div class="col-right">

      </div>
    </div>

    <div class="footer_down">

    </div>
  </footer>
  
</template>

<script>
export default {
  name: 'FooterComp',
  data(){
    return{
      dccomics:[
        {
          text:'Characters',
          url:'/',
          flag:'false'
        },
        {
          text:'Comics',
          url:'/',
          flag:'false'
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
          text:'Games',
          url:'/',
          flag:'false'
        },
        {
          text:'Videos',
          url:'/',
          flag:'false'
        },
        {
          text:'News',
          url:'/',
          flag:'false'
        },
      ],
      shops:[
        {
          text:'Shop DC',
          url:'/',
          flag:'false'
        },
        {
          text:'Shop DC Collectibles',
          url:'/',
          flag:'false'
        },
      ],
      dcs:[
        {
          text:'Terms Of Use',
          url:'/',
          flag:'false'
        },
        {
          text:'Privacy policy (New)',
          url:'/',
          flag:'false'
        },
        {
          text:'Ad Choices',
          url:'/',
          flag:'false'
        },
        {
          text:'Advertising',
          url:'/',
          flag:'false'
        },
        {
          text:'jobs',
          url:'/',
          flag:'false'
        },
        {
          text:'Subscriptions',
          url:'/',
          flag:'false'
        },
        {
          text:'Talent Workshops',
          url:'/',
          flag:'false'
        },
        {
          text:'CPSC Certificates',
          url:'/',
          flag:'false'
        },
        {
          text:'Ratings',
          url:'/',
          flag:'false'
        },
        {
          text:'Shop Help',
          url:'/',
          flag:'false'
        },
        {
          text:'Contact Us',
          url:'/',
          flag:'false'
        },
      ],
      sites:[
        {
          text:'DC',
          url:'/',
          flag:'false'
        },
        {
          text:'MAD Magazine',
          url:'/',
          flag:'false'
        },
        {
          text:'DC Kids',
          url:'/',
          flag:'false'
        },
        {
          text:'DC Universe',
          url:'/',
          flag:'false'
        },
        {
          text:'DC Power Visa',
          url:'/',
          flag:'false'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

  footer{
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    .col-left{
      display: flex;
      width: 40%;
      padding-top: 20px;
      div{
        flex-basis: calc(100% / 3);
      }
    }
  }

  h3{
    text-transform: uppercase;
    color: white;
    margin: 18px 0;
  }

  a{
    color: #828282;
    text-decoration: none;
  }

  li{
    margin: 5px 0;
  }

  .col-right{
    height: 100%;
    width: 50%;
    position: absolute;
    top: 0;
    right: 0;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-position: center;
  }

  .footer_down{
    height: 100px;
    background-color: #303030;
  }

  .container{
    position: relative;
    padding-bottom: 50px;
  }

</style>
<template>
  <header>
      <div class="ticket">
          <p>Starts TOMORROW! Our biggest event of the year..</p>
          <i class="far fa-clock"></i>
          <h3>00: 00: 00: 00</h3>
          <button>Get ticket</button>
      </div>
      <div class="menu contenitore-bg">
          <div class="logo">
              <img src="../assets/img/dark-logo.png" alt="">
          </div>
          <div class="lista">
                <ul>
                    
                    <VoceMenu
                    v-for="(voceMenu, index) in this.vociMenu"
                    :key="index"
                    :voce="voceMenu"
                    />
                    
                </ul>
          </div>
          <div class="social">
                <ul>
                    <li>
                        <i class="fab fa-twitter"></i>
                    </li>
                    <li>
                        <i class="fab fa-facebook-f"></i>
                    </li>
                    <li>
                        <i class="fab fa-instagram"></i>
                    </li>
                    <li>
                        <i class="fab fa-linkedin"></i>
                    </li>
                </ul>
          </div>
      </div>
  </header>
</template>

<script>

import VoceMenu from './VoceMenu.vue';
export default {
    name: 'Header',
    components:{
        
        VoceMenu
    },
    
    data(){
        return{
            vociMenu: ['Home', 'Pages', 'Courses', 'Features', 'Blog', 'Shop'],
        }
    }
}
</script>

<style lang="scss">
@import '../assets/style/general.scss';
@import '../assets/style/utilities.scss';
@import '../assets/style/mix.scss';
header{
    
    .ticket{
        background-color: #F5F5F5;
        height: 50px;
        @include center();
        h3{
            margin-right: 15px;
            color: #696969;
        }
        i{
            margin: 0px 5px 0px 10px;
        }
        p{
            font-size: 12px;
        }
       
    }
    .menu{
        height: 60px;
        
        @include center(between);
        .logo{
            height: 20px;
            width: 10%;
            margin-left: 20px;
            background-color: #fff;
        }
        .lista{
            height: 20px;
            li{
                margin: 0px 20px;
                font-size: 13px;
                color: #696969;
            }
            background-color: #fff;
        }
        .social{
            color: #696969;
            height: 20px;
            margin-right: 20px;
            background-color: #fff;
        }
    }
}
</style>
<template>
  <header>
      <div class="ticket">
          <p>lorem</p>
          <h2>timer</h2>
          <button>click</button>
      </div>
      <div class="menu">
          <div class="logo">
              <img src="../assets/img/dark-logo.png" alt="">
          </div>
          <div class="lista"></div>
          <div class="social"></div>
      </div>
  </header>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import '../assets/style/general.scss';
@import '../assets/style/utilities.scss';
@import '../assets/style/mix.scss';
header{
    background-color: red;
    height: 120px;
    .ticket{
        background-color: yellow;
        height: 50px;
        @include center();
        h2{
            margin: 0px 15px;
        }
    }
    .menu{
        height: 50px;
        background-color: green;
        @include center(between);
        .logo{
            height: 20px;
            width: 15%;
            background-color: #fff;
        }
        .lista{
            height: 20px;
            width: 40%;
            background-color: #fff;
        }
        .social{
            height: 20px;
            width: 15%;
            background-color: #fff;
        }
    }
}
</style>
<template>
  <section class="jumbotrone">
    <img class="paint" src="../assets/img/artist-hero-image-02.jpg" alt="">
    <img class="monkey" src="../assets/img/artist-hero-image-01.jpg" alt="">
    <img class="profile" src="../assets/img/artist-hero-image-03.png" alt="">
    <img class="bg-1" src="../assets/img/artist-shape-02-768x415.png" alt="">
    <img class="bg-2" src="../assets/img/artist-shape-01-600x577.png" alt="">
    <img class="bg-3" src="../assets/img/artist-shape-05.png" alt="">
    <img class="bg-4" src="../assets/img/artist-shape-04.png" alt="">
    <img class="bg-5" src="../assets/img/maxcoach-shape-12-150x150.png" alt="">
    <img class="bg-6" src="../assets/img/artist-shape-03.png" alt="">
    <div class="testo">
        <h1>Hello, Im Martin</h1>
        <h1>Artist Coaching And Mentoring Might Be For You</h1>
        <button>Get started tooday</button>
    </div>
      
    <img class="boy" src="../assets/img/artist-hero-image-04.jpg" alt="">
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import '../assets/style/general.scss';
@import '../assets/style/utilities.scss';
@import '../assets/style/mix.scss';
.jumbotrone{
    position: relative;
    background-color: #FCFAF7;
    padding: 50px 0px;
    height: 410px;
    @include center();
    flex-direction: row;
    img{
        width: 10%;
        position: absolute;
    }
    .monkey{
        z-index: 5;
        width: 8%;
        bottom: 35px;
        left: 93px;
    }
    .paint{
        z-index: 4;
        width: 11%;
        top: 58px;
        left: 205px;
    }
    .profile{
        width: 9%;
        top: 200px;
        left: 283px;
    }
    .bg-1{
        width: 40%;
        top: 0px;
        left: 0px;
    }
    .bg-2{
        width: 28%;
        top: 0px;
        right: 100px;
    }
    .bg-5{
        width: 7%;
        bottom: 25px;
        right: 225px;
    }
    .bg-6{
        width: 13%;
        top: 90px;
        left: 25px;
    }
    .boy{
        width: 13%;
        bottom: 35px;
        right: 150px;
    }
    .bg-3{
        width: 14%;
        bottom: 0px;
        right: 70px;
    }
    .bg-4{
        width: 5%;
        top: 40px;
        right: 105px;
    }
    .testo{      
        @include center();
        flex-direction: column;
        width: 50%;
        text-align: center;
       
    }
}
</style>
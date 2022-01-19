
<template>
  <div class="Download-wrapper">
    <div class="wrapper-container">
      <h3>Download our</h3>
      <h2>Ordering App</h2>
    <div class="app-button-wrapper">
      <a href="">
        <img src="../assets/images/app-store-badge.png" alt="">
      </a>
      <a href="">
        <img src="../assets/images/play-store-badge.png" alt="">
      </a>
    </div>
    </div>
      
  </div>
</template>

<script>
export default {
  name: "BannerDownload",

};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/general.scss';
@import '../assets/style/variables.scss';
.Download-wrapper{
    width:100%;
    background-image: url('../assets/images/app-ordering-scaled.jpg');
    background-size: 100%;
    background-repeat: no-repeat;
    // test
    height: 800px;
    // gradiente con curva
    .wrapper-container{
      padding-top: 200px;
          h3{
        font-weight: inherit;
        font-size: 50px;
            }
          h2{
            color:$GoldenRod;
            font-size: 80px;
            font-weight: inherit;
          }
    .app-button-wrapper{
      margin-top:90px;
        a{
          margin-right:30px;
          img{
          width:200px;  
          }
        }
    }
    }
}
</style>
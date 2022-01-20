<template>
  <div class="wrapper-container jumbo">
      <div class="jumbo-footer-menus">

          <div class="jumbo-footer-description">
                  <span class="icon"><i class="far fa-clock"></i></span><span>24/7 DELIVERY</span>
          </div>
          <div class="jumbo-footer-description">
                  <span class="icon"><i class="fas fa-hamburger"></i></span><span>OVER 100 DISHES</span>
          </div>
          <div class="jumbo-footer-description">
                  <span class="icon"><i class="fas fa-mobile-alt"></i></span><span>IN APP ORDERING</span>
          </div>
          <div class="jumbo-footer-description">
                  <span class="icon"><i class="fas fa-car"></i></span><span>FAST DELIVERY</span>
          </div>

      </div>


  </div>
</template>

<script>
export default {
  name: "JumboFooter",

};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/general.scss';
.jumbo{
position: absolute;
bottom:-140px;
left:50%;
right: 50%;
transform: translate(-50%, -50%);
}
.jumbo-footer-menus{
    height: 140px;
background-color: white;
                display: flex;
                justify-content: space-around;
                margin-left: 40px;
                .jumbo-footer-description{
                    line-height: 140px;
                    span{
                        font-size: 20px;
                    }
                    .icon{
                        margin-right:15px;
                    }
}


}
</style>
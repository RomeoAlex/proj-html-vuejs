<template>
<div class="wrapper-container">
  <div class="jumbo-text-wrapper">
      <div class="jumbo-text">
      <h3>Hungry?</h3>
        <h2>Great Food</h2>
        <h2>Delivered</h2>
      </div>
      <button class="primary">VIEW OUR MENU <i class="fas fa-arrow-circle-right"></i></button>      
  </div>
</div>

</template>

<script>
export default {
  name: "JumboText",

};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/variables.scss';
@import '../assets/style/general.scss';
.jumbo-text-wrapper{
    position: absolute;
    top:40%;
    
    .jumbo-text{
    color: white;
    font-weight: 900;
    h3{
        font-weight: inherit;
        font-size: 50px;
    }
    :nth-child(2){
        color:$GoldenRod;
    }
    h2{
       font-size: 90px;
       font-weight: inherit;
    }
    }
}

</style>
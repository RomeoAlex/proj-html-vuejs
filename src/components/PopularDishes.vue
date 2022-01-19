<template>
<div class="wrapper-container popular">
  <h2>Our Most Popular Dishes</h2>
  <div class="popular-wrapper">
      <div class="popular-card">
          <!-- v-for su data -->
      </div>
        <button>START YOUR ORDER</button>
  </div>
</div>

</template>

<script>
export default {
  name: "PopularDishes",

};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/general.scss';
.popular{
  margin-top:140px;
  text-align: center;
  h2{
    font-size: 50px;
    }
  .popular-wrapper{
    
    .popular-card{

    }
  }
}
</style>

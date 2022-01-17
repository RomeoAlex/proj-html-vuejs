<template>
  <div class="popular-wrapper">
      <h2>Our Most Popular Dishes</h2>
      <div class="popular-card">
          <!-- v-for su data -->
      </div>
        <button>START YOUR ORDER</button>
  </div>
</template>

<script>
export default {
  name: "PopularDishes",

};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.popular-wrapper{
    width:60%;
    margin: auto;
    // test
    height: 600px;

}
</style>

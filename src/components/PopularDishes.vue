<template>
<div class="wrapper-container popular">
  
  <div class="popular-wrapper">
    <h2>Our Most Popular Dishes</h2>
      <div class="popular-cards">
          <DishesCard v-for="(dish, index)  in dishes " :key="index" :details="dish"/>
      </div>
        <button>START YOUR ORDER</button>
  </div>
</div>

</template>

<script>
import DishesCard from "./DishesCard.vue";
export default {
name: "PopularDishes",
  components: {
    DishesCard,
  },
  data: function() {
      return {
          dishes: [
                    {        
                        image: 'skin-on-fries.jpg',
                        name: 'Skin On Fries',
                        price: '$3.00 - $6.00',
                    },
                    {        
                        image: 'choco-cookie-frappe.jpg',
                        name: 'Choco Cookie Frappe',
                        price: '$4.99',
                    },
                    {        
                        image: 'donut-burger.jpg',
                        name: 'The Donut Burger',
                        price: '$6.99',
                    }, 
                ],
            };
        },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/general.scss';
.popular{
  margin-top:140px;
  text-align: center;
  margin-bottom: 100px;
  .popular-wrapper{
    width:100%;
    h2{
    font-size: 50px;
    }
    
    .popular-cards{
      width: 100%;
      margin: auto;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
    }
  }
}
</style>

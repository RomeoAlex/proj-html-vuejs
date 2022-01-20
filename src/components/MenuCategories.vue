<template>
<div class="wrapper-container categories">
  <div class="categories-wrapper">
      <button class="primary">VIEW THE FULL MENU <i class="fas fa-arrow-circle-right"></i></button>
      <h2>Menu Categories</h2>
      <div class="categories-card">
        <FoodCategoriesCard v-for="(food, index)  in foodCategories " :key="index" :details="food"/>
          
      </div>
    <!-- sub categories menu -->
  </div>
</div>
</template>

<script>
import FoodCategoriesCard from "./FoodCategoriesCard.vue";
export default {
  name: "MenuCategories",
  components: {
    FoodCategoriesCard,
  },
  data: function() {
      return {
          foodCategories: [
                    {        
                        image: 'appetizers-menu-background.jpg',
                        name: 'Appetizers',
                        url: '#',

                    },
                    {        
                        image: 'burgers-menu-background.jpg',
                        name: 'Burgers',
                        url: '#',
                    },
                    {        
                        image: 'pizza-menu-background.jpg',
                        name: 'Pizzas',
                        url: '#',
                    },
                    {        
                        image: 'fries-menu-background.jpg',
                        name: 'Fries',
                        url: '#',
                    },
                    {        
                        image: 'sides-menu-background.jpg',
                        name: 'Sides',
                        url: '#',
                    },
                    {        
                        image: 'desserts-menu-background.jpg',
                        name: 'Desserts',
                        url: '#',
                    },
                    {        
                        image: 'beverages-menu-background.jpg',
                        name: 'Beverages',
                        url: '#',
                    },
                    {        
                        image: 'specials-menu-background.jpg',
                        name: 'Specials',
                        url: '#',
                    }, 
                ],
            };
        },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/general.scss';
  .categories{
    padding: 30px;    
  .categories-wrapper{
    margin:50px 0 ;
    width:100%;
    h2{
    font-size: 50px;
    }
    button{
      float:right;
    }
    
    .categories-card{
      padding-top: 50px;
      width: 100%;
      margin: auto;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;

    }
  }
  }

</style>

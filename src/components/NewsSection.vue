<template>
<div class="wrapper-container news">
    <div class="news-wrapper">
      <button class="primary">READ MORE NEWS</button>
      <h2>Latest News</h2>
      
      <div class="news-card">
          <NewsCard v-for="(news, index)  in newsCollection " :key="index" :details="news"/>
      </div>

  </div>
</div>

</template>

<script>
import NewsCard from "./NewsCard.vue";
export default {
  name: "NewsSection",
  components: {
    NewsCard,
  },
  data: function() {
      return {
          newsCollection: [
                    {        
                        image: 'pancake-burger.jpg',
                        title: 'NEW: The Pancake Burger',
                        description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque ipsa sed nam esse repellendus doloremque debitis commodi molestias fugit sint quo architecto odit, doloribus nihil molestiae expedita ut pariatur quos.',
                        url:'#',
                    },
                    {        
                        image: 'new-milkshake-menu.jpg',
                        title: 'New Milkshake Menu',
                        description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque ipsa sed nam esse repellendus doloremque debitis commodi molestias fugit sint quo architecto odit, doloribus nihil molestiae expedita ut pariatur quos.',
                        url:'#',
                    },

                ],
            };
        },
};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/general.scss';
  .news{
      padding:50px 0;
  .news-wrapper{
    width:100%;

    h2{
    font-size: 50px;
    }
    button{
      float:right;
    }
    .news-card{
      width: 100%;
      margin: auto;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;

    }
  }
  }

</style>
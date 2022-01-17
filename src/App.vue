<template>
  <div id="app">
    <Jumbotron />
    <PopularDishes />
    <BannerDiscount />
    <MenuCategories />
    <BannerDownload />
    <NewsSection />
    <Footer />
  </div>
</template>

<script>
import Jumbotron from "./components/Jumbotron.vue";
import PopularDishes from "./components/PopularDishes.vue";
import BannerDiscount from "./components/BannerDiscount.vue";
import MenuCategories from "./components/MenuCategories.vue";
import BannerDownload from "./components/BannerDownload.vue";
import NewsSection from "./components/NewsSection.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",
  components: {
    Jumbotron, PopularDishes, BannerDiscount, MenuCategories, BannerDownload, NewsSection, Footer,
  },
};
</script>

<style lang="scss">
@import url('./assets/style/general.scss');
#app {

}
</style>

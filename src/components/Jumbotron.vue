<template>
  <div class="jumbotron-wrapper">
    <Header />
    <SideBar />
    <JumboText />
    <JumboFooter />
    
  </div>
</template>

<script>
import Header from "./Header.vue";
import SideBar from "./SideBar.vue";
import JumboText from "./JumboText.vue";
import JumboFooter from "./JumboFooter.vue";
export default {
  name: "Jumbotron",
  components: {
    Header, SideBar, JumboText, JumboFooter,
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.jumbotron-wrapper{
    width:100%;
    background-image: url('../assets/images/home-background-hero-scaled.jpg');
    background-size: 100%;
    background-repeat: no-repeat;
    // test
    height: 1100px;
    position:relative;
    
}
</style>

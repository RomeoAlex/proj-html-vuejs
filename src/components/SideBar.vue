<template>
  <div class="side-wrapper">
      <div class="side-menus">
          <div class="user-log">
              <a href="#"><i class="fas fa-plus"></i></a>

          </div>
      </div>
      <div class="showcase-icon">
          <a href=""></a>
          <a href=""></a>

      </div>

  </div>
</template>

<script>
export default {
  name: "SideBar",

};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/variables.scss';
.side-wrapper{
    position:absolute;
    top:10px;
    right:10px;
    
    // test
    // height: 500px;
    // width:200px;
    // background-color: chartreuse;
    .side-menus{
        margin-top: 30px;
        display: flex;
        flex-direction: column;
        .user-log a{
            text-decoration: none;
            font-size: 20px;
            background-color: $RedCardinal;
            color:white;
            padding:25px;
            border-radius: 50%;
        }
        .showcase-icon{

            a{
                padding:20px;
                background-color: white;
                border-radius: 5%;
            }
        }
    }

}
</style>
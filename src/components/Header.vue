<template>
<div class="wrapper-container">
    <header>
        <div class="header-container">
                <div class="logo">
                    <img src="../assets/images/takeout-logo.png" alt="Logo AVADA TAKEOUT">
                    
                </div>
                <div class="nav-bar">
                    <ul class="menu">
                        <li v-for="(link , index) in links" :key="index">
                            <a :class="{ 'current' :link.current }" href="link.url" >{{ link.text }} </a>
                        </li>
                        <li>
                            <a href="#" id="cart-shop"><i class="fas fa-shopping-cart"></i></a>
                        </li>
                    </ul>
                </div>  
        </div>
        
    </header>
</div>

</template>

<script>
export default {
  name: "Header",
  data: function() {
      return {
          links: [
                    {        
                        text: 'Home',
                        url: '#',
                        icon:`<i class="fas fa-angle-down"></i>`,
                        current: true,
                    },
                    {
                        text: 'Order Online',
                        url: '#',
                        current: false,
                    },
                    {
                        text: 'About',
                        url: '#',
                        current: false,
                    },
                    {
                        text: 'News',
                        url: '#',
                        current: false,
                    },
                    {
                        text: 'Contact Us',
                        url: '#',
                        current: false,
                    },
                    
                ],
            };
        },
};
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
.header-container{
        padding: 0 20px;
        height:140px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        // test
        // background-color:red;
        // line-height: 180px;
        .logo{
                img{
                    
                    }
        }
        .nav-bar{
                .menu{
                    display: flex;
                        li{
                            font-size: 20px;
                            margin-left: 35px;
                            font-weight: bold;
                        }
                        a{
                            text-decoration: none;
                            line-height: 136px;
                            display: inline-block;
                            color:white;
                                &.current{
                                color:$GoldenRod;
                                
                                }
                        }
                        #cart-shop{
                            color: white;
                        }
                        
                }
        }
        
}
</style>
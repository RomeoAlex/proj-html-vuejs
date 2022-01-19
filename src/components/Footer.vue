<template>
  <div class="Footer-wrapper">
      <div class="footer-menus">
        <ul >
          <li>
            ORDER ONLINE
          </li>
          <li v-for="(food, index)  in foodCategories " :key="index" :details="food" class="footer-list">
            <a :href="food.url">{{food.name}}</a>
          </li>
        </ul>
        <ul>
          <li>
            NAVIGATE
          </li >
          <li v-for="(link , index) in links" :key="index" class="footer-list">
            <a :class="{ 'current' :link.current }" href="link.url" >{{ link.text }} </a>
          </li>
          
        </ul>
        <ul>
          <li>
            INFORMATION
          </li>
          <li class="footer-list">
            <a href="#">My Account</a>
          </li>
          <li class="footer-list">
            <a href="#">Terms of Service</a>
          </li>
          <li class="footer-list">
            <a href="#">Privacy Policy</a>
          </li>
        </ul>
        <ul>
          <li>
            OPENING HOURS
          </li >
          <li v-for="(open , index) in openings" :key="index" class="openings-list">
            <span>{{open.day}}  - <span class="openings"> {{open.hours}} to {{open.hours1}}</span></span>
          </li>
        </ul>
        <div class="coupon-section">
            <span>VOUCHER</span>
            <img src="../assets/images/footer-coupon.png" alt="coupon image">
            <h3>Just Use the Code</h3>
            <h2>FIRST ORDER</h2>
            <h3>at Checkout</h3>
        </div>

      </div>
          <div class="sub-footer">
                <img src="../assets/images/takeout-logo.png" alt="">
                <Subscribe />
                <div class="social-icons">
                    <span v-for="(social , index) in socials" :key="index">
                      <a :href="social.url">
                        <i :class="social.icon"></i>
                      </a>
                    </span>
                    
                </div>
                <p>Copyright</p>
          </div>
  </div>
</template>

<script>
import Subscribe from "./Subscribe.vue";
export default {
 
  name: "Footer",
  components:{Subscribe,
  }, 
 data: function() {
      return {
          foodCategories: [
                    {        
                        image: 'appetizers-menu-background.jpg',
                        name: 'APPETIZERS',
                        url: '#',
                    },
                    {        
                        image: 'burgers-menu-background.jpg',
                        name: 'BURGERS',
                        url: '#',
                    },
                    {        
                        image: 'pizza-menu-background.jpg',
                        name: 'PIZZAS',
                        url: '#',
                    },
                    {        
                        image: 'fries-menu-background.jpg',
                        name: 'FRIES',
                        url: '#',
                    },
                    {        
                        image: 'sides-menu-background.jpg',
                        name: 'SIDES',
                        url: '#',
                    },
                    {        
                        image: 'desserts-menu-background.jpg',
                        name: 'DESSERTS',
                        url: '#',
                    },
                    {        
                        image: 'beverages-menu-background.jpg',
                        name: 'BEVERAGES',
                        url: '#',
                    },
                    {        
                        image: 'specials-menu-background.jpg',
                        name: 'SPECIALS',
                        url: '#',
                    }, 
                ],
            links: [
                    {        
                        text: 'Home',
                        url: '#',
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
            openings:[
                    {        
                        day: 'Mon',
                        hours: '10AM',
                        hours1:'11PM'
                    },
                    {
                        day: 'Home',
                        hours: '10AM',
                        hours1:'11PM'
                    },
                    {
                        day: 'Home',
                        hours: '10AM',
                        hours1:'11PM'
                    },
                    {
                        day: 'Home',
                        hours: '10AM',
                        hours1:'11PM'
                    },
                    {
                        day: 'Home',
                        hours: '10AM',
                        hours1:'11PM'
                    },
                                        {
                        day: 'Home',
                        hours: '10AM',
                        hours1:'11PM'
                    },
                    {
                        day: 'Home',
                        hours: '10AM',
                        hours1:'11PM'
                    },    
                ],
            socials: [
                {
                  icon:'fab fa-facebook-f',
                  url:'#',
                },
                {
                  icon:'fab fa-twitter',
                  url:'#',
                },
                {
                  icon:'fab fa-instagram',
                  url:'#',
                },
                {
                  icon:'fab fa-linkedin-in',
                  url:'#',
                },
                {
                  icon:'',
                  url:'#',
                },
                {
                  icon:'fab fa-youtube',
                  url:'#',
                },
                {
                  icon:'far fa-envelope',
                  url:'#',
                },
                ],        
          };
        },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/variables.scss';
.Footer-wrapper{
    width:100%;
    background-image: url('../assets/images/footer-background-scaled.jpg');
    background-size: 100%;
    background-repeat: no-repeat;
    // test
    height: 1500px;
                .footer-menus{
                  padding-top:40px;
                    width: 80%;
                    margin:auto;
                    display: flex;
                    flex:wrap;
                    justify-content: space-between;
                                ul{
                                  width:calc(100% / 5);
                                  list-style: none;
                                            :first-child{
                                              margin-bottom:20px;
                                              }
                                          .footer-list{
                                          padding:10px 0;
                                          }
                                          .openings-list{ padding:5px 0;}
                                        li{
                                            
                                          color: white;
                                                    span{
                                                      color: white;
                                                      .openings{
                                                        color:$GoldenRod;
                                                                }
                                                        }
                                                  a{
                                                    text-decoration: none;
                                                    color: white;
                                                    text-transform: capitalize;
                                                    .current{
                                                      color:$GoldenRod;
                                                  }
                                                  }

                                        
                                }
                    
                    }
                    .coupon-section{
                      width:calc(100% / 6);
                      color: white;
                      text-align: center;
                    img{
                      width:100%;}
                      h2{color:$GoldenRod;}
                                        }

                    }
                    .sub-footer{
                      padding-top: 50px;
                      text-align: center;

                    }
                    .social-icons{
                      margin-top: 50px;
                      a{
                        font-size: 30px;
                        padding:30px;
                        color: white;
                      }
                    }

}
</style>
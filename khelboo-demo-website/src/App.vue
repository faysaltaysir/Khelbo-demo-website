<template>
  <!-- <h1>W3 school</h1> -->
  <nav-bar
    :sections="sections"
  ></nav-bar> 
  <bethe-part></bethe-part>
  <search-turf></search-turf>
  <cards-view></cards-view>
   <image-view></image-view>
   <news-letter></news-letter>
   <footer-view></footer-view>
</template>
<script>
import NavBar from './components/navbar.vue'
import BoDy from './components/Body.vue'
import SearchTurf from './components/Search-turf.vue';
import CardsView from './components/cards.vue' 
import RegisterView from './components/Register.vue'
import ImageView from './components/Image.vue'
import FooterView from './components/Footer.vue'
import NewsLetter from './components/News.vue'
import BethePart from './components/BeThePart.vue'
export default{
  components: {
    NavBar,BoDy,SearchTurf,CardsView,RegisterView,ImageView,FooterView,NewsLetter,BethePart
  },
  data(){
    return{
      sections: [
      {
          key:1,
          name:'Home'
      },
      {
          key:2,
          name:'Book A Venue'
      },
      {
          key:3,
          name:'Turfs'
      },
      {
          key:4,
          name:'Turnaments'
      },
      {
          key:5,
          name:'About Us'
      },
      {
          key:6,
          name:'Contact Us'
      }
      ],
      
      
    }
  }
}


</script>


<style>

.racing-sans-one-regular {
        font-family: "Racing Sans One", sans-serif;
        font-weight: 900;
        font-style: bold;
        font-style: italic;
    }
  body{
    margin: 0px;
    padding: 0px;
    font-size: 16px;
  }
  .poppins-thin {
    font-family: "Poppins", sans-serif;
    font-weight: 200;
    font-style: normal;
  }
  .poppins-thick {
    font-family: "Poppins", sans-serif;
    font-weight: 600;
    font-style: normal;
    /* font-size: 1.9vw; */
  }
    
  
</style>

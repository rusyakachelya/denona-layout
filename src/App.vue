<template>
  <div id="app">
    <v-header/>
    <v-new-product
      :newProducts="newProducts"
    />
    <v-about/>
    <v-slider
      :sliderImg="sliderImg"
    />
    <v-advice/>
    <v-footer/>
  </div>
</template>

<script>
import vHeader from '@/components/Header/v-header.vue'
import VNewProduct from '@/components/NewProduct/v-newProduct.vue'
import vAbout from '@/components/About/v-about.vue'
import vSlider from '@/components/Slider/v-slider.vue'
import vAdvice from '@/components/Advices/v-advice.vue'
import VFooter from '@/components/Footer/v-footer.vue'


import New1 from '@/assets/images/new-1.png'
import New2 from '@/assets/images/new-2.png'
import New3 from '@/assets/images/new-3.png'

import Slide1 from '@/assets/images/slide-1.png'
import Slide2 from '@/assets/images/slide-2.png'
import Slide3 from '@/assets/images/slide-3.png'



export default {
  name: 'App',
  components: {
    vHeader,
    VNewProduct,
    vAbout,
    vSlider,
    vAdvice,
    VFooter
    
  },
  data() {
    return {
        newProducts: [
          {img: New1, title: 'HY-GEN PRIMER SERUM',id:1},
          {img: New2, title: 'I NEED A ROSE LIPSTICK',id:2},
          {img: New3, title: 'RETRO EYESHADOW PALETTE',id:3},
        ],
        sliderImg: [
          {img:Slide1,id:1},
          {img:Slide2,id:2},
          {img:Slide3,id:3},
        ]
    }
  }
}
</script>

<style>
  .container{
    max-width: 1200px;
    padding: 0 15px;
    margin: 0 auto;
  }
  #app{
    background: #121212;
  }
  p{
    margin: 0px;
  }
  h6{
    margin: 0;
  }
</style>

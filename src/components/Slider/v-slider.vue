<template>
    <div class="v-slider">
        <div class="container">
             <h4 class="slider__title">Найпопулярніші продукти</h4>
             <div class="slider__box">
                <carousel 
                    class="slider"
                    :perPage="2"
                    :paginationEnabled="true"
                    :navigationEnabled="true"
                    :navigation-next-label="nextLabel"
                    :navigation-prev-label="prevLabel"
                >  
                <slide
                    class="slide"
                    v-for="slide in sliderImg"
                    :key="slide.id"
                >
                    <img 
                    :src="slide.img"
                    >
                </slide>
            </carousel>
             </div>
           <div class="slider__link"><a class="" href="">Купити онлайн</a></div>
        </div>
    </div>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel';

import NextBtn from '@/assets/images/next-btn.png'
import PrevBtn from '@/assets/images/prev-btn.png'

export default {
    name: 'vSlider',
    components: {
    Carousel,
    Slide
  },
  props: {
    sliderImg:{
        type: Array,
        require: true,
    }
  },
  data () {
    return {
        nextLabel: `<img src='${NextBtn}'/>`,
        prevLabel:  `<img src='${PrevBtn}'/>`
    }
  },
}


</script>

<style>
    .slider__title{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 500;
        font-size: 36px;
        line-height: 44px;
        color: #EC008C;
        margin-bottom: 55px;
        text-align: center;
    }
    .slider__box{
        max-width: 900px;
        text-align: center;
        margin: 0 auto;  
    }
    .slider__link{
        padding: 16px 19px;
        font-family: 'Roboto';
        font-style: normal;
        font-weight: 700;
        font-size: 18px;
        line-height: 21px;
        border: 3px solid #EC008C;
        max-width: 130px;
        margin: 0 auto;
        color: #EC008C;
    }
    .slider__link a{
         color: #EC008C;
    }
    .VueCarousel-pagination{
        margin-bottom: 30px;
    }
    .VueCarousel-navigation-next[data-v-453ad8cd] {
    right: 30px;
    transform: translateY(-50%) translateX(100%);
    font-family: "system";
    top: 155px;
    } 
    .VueCarousel-navigation-prev[data-v-453ad8cd] {
    left: 30px;
    transform: translateY(-50%) translateX(-100%);
    font-family: "system";
    top: 155px;
}
</style>
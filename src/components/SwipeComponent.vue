<template>
    <div class="swiper-template">
        <div class="swipe-title">
            <h1>Мероприятия</h1>
        </div>
        <swiper
        ref="{swiperRef}"
        :slides-per-view="count"
    :space-between="16"
    :loop="true"
    :modules="modules"
    :class="MySwiper"

        >
            <swiper-slide >
                <div class="img"><img src="../assets/images/Frame 811332.png" alt="img"></div>    
            </swiper-slide>
            <swiper-slide>
                <div class="img"><img src="../assets/images/Frame 811333.png" alt="img"></div>    
            </swiper-slide><swiper-slide>
                <div class="img"><img src="../assets/images/Frame 811332.png" alt="img"></div>    
            </swiper-slide>
            <swiper-slide >
                <div class="img"><img src="../assets/images/Frame 811333.png" alt="img"></div>    
            </swiper-slide>
            
        </swiper>
      
    </div>
</template>

<script>
  import { Swiper, SwiperSlide } from 'swiper/vue';
  import 'swiper/css'
  import 'swiper/css/navigation';
  import '../style.css'
  import {Navigation } from 'swiper/modules'

    export default {
        name:"SwipeComponent",
        components:{
            Swiper,
      SwiperSlide,
        },
        data() {
        return {
            screenWidth: window.innerWidth,
            count: 1
        };
    },
    mounted() {
        window.addEventListener("resize", this.onResize);
    },
    beforeUnmount() {
        window.removeEventListener("resize", this.onResize);
    },
    methods: {
        onResize() {
            this.screenWidth = window.innerWidth;
            if (this.screenWidth > 430) {
                this.count = 3
            }
            else {
                this.count = 2
            }
        }
    },
        setup() {
      return {
        modules:[Navigation]
      };
    },
    
    }
   
</script>

<style  scoped>
.swiper-template{
    margin-top: 48px;
    position: relative;
}
.swipe-title{
    margin-bottom: 20px;
}

.img{
    border-radius: 16px !important;
    margin-top: 60px;
}
@media only screen and (max-width: 430px) {
    .img{
        margin-top: 20px;
        height: 216px;
    }
    .swiper-template{
    margin-top: 20px;

    }
}
</style>
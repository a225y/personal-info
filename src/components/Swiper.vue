<template>
    <div class="main">
            <swiper
                class="mySwiper"
                :spaceBetween="30"
                :centeredSlides="true"
                :autoplay="{
                delay: 3400,
                disableOnInteraction: false,
                }"
                :pagination="{
                clickable: true,
                }"
                :navigation="true"
                :modules="modules"
            >
    
            <swiper-slide class=" el">
                <img src="../assets/01.jpg">
            </swiper-slide>
            <swiper-slide class=" el">
                <img src="../assets/02.jpg">
            </swiper-slide>
            <swiper-slide class=" el">
                <img src="../assets/03.jpg">
            </swiper-slide>
            <swiper-slide class=" el">
                <img src="../assets/04.jpg">
            </swiper-slide>
            <swiper-slide class=" el">
                <img src="../assets/05.jpg">
            </swiper-slide>
        </swiper>
    </div>
</template>
<script>
import { Swiper,SwiperSlide } from 'swiper/vue';
import 'swiper/css'
import 'swiper/css/pagination';
import 'swiper/css/navigation';
import { Autoplay,Pagination,Navigation} from 'swiper/modules';

export default{
    components:{
        Swiper,
        SwiperSlide,
    },
    setup(){
        return {
            modules:[Autoplay,Pagination,Navigation],
        }
    }
}

</script>
<style scoped>
    .main{
        background-color: #000;
    }
    .main img{
        width: 100%;
        max-height: 450px;
        background-color: #8ea69b;
    }
</style>
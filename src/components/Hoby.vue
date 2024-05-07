<template>
    <div class="main">
        <swiper class="mySwiper" :spaceBetween="30" :centeredSlides="true" :autoplay="{
                delay: 3800,
                disableOnInteraction: false,
                }" :pagination="{
                clickable: true,
                }" :navigation="true" :modules="modules">

            <swiper-slide class=" el">
                <img src="../assets/06.jpg">
            </swiper-slide>
            <swiper-slide class=" el">
                <img src="../assets/07.jpg">
            </swiper-slide>
            <swiper-slide class=" el">
                <img src="../assets/08.jpg">
            </swiper-slide>
            <swiper-slide class=" el">
                <img src="../assets/09.jpg">
            </swiper-slide>
            <swiper-slide class=" el">
                <img src="../assets/10.jpg">
            </swiper-slide>
            <swiper-slide class=" el">
                <img src="../assets/11.jpg">
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
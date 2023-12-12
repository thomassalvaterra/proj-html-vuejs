<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/modules';
import 'swiper/css/bundle';

import 'swiper/css/pagination';
import 'swiper/css/navigation';
import { Navigation, Autoplay, Pagination } from 'swiper/modules';

export default {
    name: "PageJumbo",
    components: {
        Swiper,
        SwiperSlide
    },

    setup() {
        return {
            modules: [Navigation, Autoplay, Pagination],
        };
    },

    methods: {},
    mounted() { }
}
</script>

<template>
    <div class="jumbotron">
        <swiper :autoplay="{
            delay: 7000,
            disableOnInteraction: false,
        }" :pagination="{
    clickable: true,
}" :navigation="true" :modules="modules" class="mySwiper position-relative">
            <swiper-slide><img src="../assets/img/slider.jpg" alt=""></swiper-slide>
            <swiper-slide><img src="../assets/img/slider-2.jpg" alt=""></swiper-slide>
        </swiper>
        <div class="d-flex justify-content-center">
            <div class="w-25 text-center position-absolute bottom-50 left-50">
                <h6><b>Welcome To Our Movie Site</b></h6>
                <h1>OUR SPECIAL <span class="cl-green">MOVIES</span></h1>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Maxime repudiandae perspiciatis, dolores, nisi
                    quis
                    beatae
                    soluta, amet quos ratione tempore a quas ut eos dolor. Sequi suscipit odit reiciendis nesciunt!
                </p>
                <button type="button" class="btn btn-outline-success">Read More</button>
            </div>
        </div>
    </div>
</template>

<style scoped>
.cl-green {
    color: rgb(19, 190, 19);
}
</style>
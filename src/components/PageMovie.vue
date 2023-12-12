<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';
// Import Swiper styles
import 'swiper/css';
export default {
    name: "PageMovie",
    components: {
        Swiper,
        SwiperSlide,
    },
    data() {
        return {
            cardInfo: [
                {
                    title: "Donec English Action Movie",
                    category: "Coming Soon",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("2 - 1(1).jpg")
                },
                {
                    title: "English Action Movie In Strack",
                    category: "Latest Movie",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "Movie Auctor Quisque In Strack",
                    category: "Top Rating",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "Auctor Movie Quisque In Strack",
                    category: "TV Series",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "Donec Movie Quisque In Strack",
                    category: "Coming Soon",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "New Movie Quisque In Strack",
                    category: "Latest Movie",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "Quisque In Strack New Movie",
                    category: "Top Rating",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "Nulla Strack New Animate Movie",
                    category: "TV Series",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "Blue Strack New Animate Movie",
                    category: "Coming Soon",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "Animate Blue Strack New Movie",
                    category: "Latest Movie",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "Hurry Animate Blue Strack New Movie",
                    category: "Top Rating",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "Quisque Auctor Movie In Strack",
                    category: "Coming Soon",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "New Movie Quisque In Strack",
                    category: "Latest Movie",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "Movie Action Garila English",
                    category: "Top Rating",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },
                {
                    title: "Action Garila English Movie",
                    category: "TV Series",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: "../assets/img/4-1.jpg"
                },

            ]
        }
    },
    methods: {
        getImagePath: function (img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <div class="border-start border-success border-bottom">
        <h2 class="mt-4 ms-4"><b>New Movie</b></h2>
        <p class="ms-4">Lorem Ipsum is simply dummy text of the printing and typesettin</p>
    </div>

    <div>
        <swiper :watchSlidesProgress="true" :slidesPerView="3" class="mySwiper">
            <swiper-slide v-for="carte in  cardInfo "><img src="../assets/img/cropped-logo.png">
                <h4>{{ carte.title }}</h4>
            </swiper-slide>
        </swiper>
    </div>
</template>

<style scoped></style>
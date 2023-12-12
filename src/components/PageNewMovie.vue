<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';
// Import Swiper styles
import 'swiper/css';
export default {
    name: "PageNewMovie",
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
                    src: this.getImagePath("2-1 (1).jpg")
                },
                {
                    title: "English Action Movie In Strack",
                    category: "Latest Movie",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("4-1.jpg")
                },
                {
                    title: "Movie Auctor Quisque In Strack",
                    category: "Top Rating",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("6.jpg")
                },
                {
                    title: "Auctor Movie Quisque In Strack",
                    category: "TV Series",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("5 (1).jpg")
                },
                {
                    title: "Donec Movie Quisque In Strack",
                    category: "Coming Soon",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("1-2.jpg")
                },
                {
                    title: "New Movie Quisque In Strack",
                    category: "Latest Movie",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("2.jpg")
                },
                {
                    title: "Quisque In Strack New Movie",
                    category: "Top Rating",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("3 (1).jpg")
                },
                {
                    title: "Nulla Strack New Animate Movie",
                    category: "TV Series",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("4.jpg")
                },
                {
                    title: "Blue Strack New Animate Movie",
                    category: "Coming Soon",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("3.jpg")
                },
                {
                    title: "Animate Blue Strack New Movie",
                    category: "Latest Movie",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("5 (1).jpg")
                },
                {
                    title: "Hurry Animate Blue Strack New Movie",
                    category: "Top Rating",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("1.jpg")
                },
                {
                    title: "Quisque Auctor Movie In Strack",
                    category: "Coming Soon",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("2.jpg")
                },
                {
                    title: "New Movie Quisque In Strack",
                    category: "Latest Movie",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("5.jpg")
                },
                {
                    title: "Movie Action Garila English",
                    category: "Top Rating",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("3.jpg")
                },
                {
                    title: "Action Garila English Movie",
                    category: "TV Series",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    src: this.getImagePath("3-1.jpg")
                },

            ]
        }
    },
    methods: {
        getImagePath: function (img) {
            return new URL(`../assets/${img}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <section class="margin">
        <div class="border-start border-success border-bottom">
            <h2 class="mt-4 ms-4"><b>New Movie</b></h2>
            <p class="ms-4">Lorem Ipsum is simply dummy text of the printing and typesettin</p>
        </div>

        <swiper :watchSlidesProgress="true" :slidesPerView="3" class="mySwiper">
            <swiper-slide v-for="carte in cardInfo ">
                <img :src="carte.src" class="rounded-4 mt-20 position-relative">
                <div class="d-flex justify-content-center">
                    <div class="position-absolute top-50 left-50 h-50">
                        <h4><b>{{ carte.title }}</b></h4>
                        <div><strong>Category: {{ carte.category }}</strong></div>
                        <div class="fs-12">Release: {{ carte.release }}</div>
                        <p class="fs-12">Genres: {{ carte.genres }}</p>
                        <div class="d-flex justify-content-between mt-45">
                            <div class="bg-col">Details</div>
                            <div class="bg-col">288 Views</div>
                        </div>

                    </div>
                </div>

            </swiper-slide>
        </swiper>
    </section>
</template>

<style scoped>
img {
    width: 100%;
    height: 400px;
}

img :hover {
    display: block;
}

.bg-col {
    background-color: rgb(6, 15, 25);
    padding: 7px;
    border-radius: 10px;
}

.mt-20 {
    margin-top: 20px;
}

.mt-45 {
    margin-top: 45px;
}

.fs-12 {
    font-size: 12px;
}

.margin {
    margin: 100px 0;
}
</style>
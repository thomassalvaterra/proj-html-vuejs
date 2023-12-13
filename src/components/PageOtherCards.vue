<script>
import { faSpoon } from '@fortawesome/free-solid-svg-icons';

export default {
    name: "PageOtherCards",

    data() {
        return {
            cardInfo: [
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
                }
            ],
            btn: [
                {
                    title: "All"
                },
                {
                    title: "Coming Soon"
                },
                {
                    title: "Latest Movie"
                },
                {
                    title: "Top Rating"
                },
                {
                    title: "TV Series"
                }
            ]
        }
    },
    methods: {
        getImagePath: function (img) {
            return new URL(`../assets/${img}`, import.meta.url).href;
        },
        search() {
            this.$emit("search");
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
        <div class="mt-4">
            <button v-for="button in btn" class="btn" @click="search">{{ button.title }}</button>
        </div>
        <div class="cardContainer d-flex flex-wrap mt-4 ">
            <div v-for="carte in cardInfo" class="cardBox position-relative">
                <div class="bg-opacity">
                    <img :src="carte.src">
                </div>
                <div class="d-flex justify-content-center">
                    <div class="position-absolute topperia">
                        <h4><b>{{ carte.title }}</b></h4>
                        <div><strong>Category: {{ carte.category }}</strong></div>
                        <div class="hide">
                            <div class="fs-12">Release: {{ carte.release }}</div>
                            <p class="fs-12">Genres: {{ carte.genres }}</p>
                        </div>
                        <div class="d-flex justify-content-between mt-45">
                            <div class="bg-col"><a href="#">Details</a></div>
                            <div class="bg-col"><a href="#">288 Views</a></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
button {
    color: white;
}

button:hover {
    color: rgb(19, 190, 19);
    border-bottom: 1px solid rgb(19, 190, 19);
}

.cardBox {
    width: calc(100% / 3 - 30px);
    margin: 10px;
}

img {
    width: 100%;
    height: 100%;
}

.topperia {
    top: 200px;
}

.bg-opacity {
    width: 100%;
    height: 400px;
    background-color: black;
    opacity: 0.2;
}

.bg-col {
    background-color: rgb(6, 15, 25);
    padding: 7px;
    border-radius: 10px;
}

.bg-col:hover {
    background-color: rgb(19, 190, 19);
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

.hide {
    display: none;
}

.margin {
    margin: 100px 0;
}

a {
    text-decoration: none;
    color: white;
}
</style>
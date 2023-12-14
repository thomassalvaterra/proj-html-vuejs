<script>
export default {
    name: "PageMoviePlaylist",
    // Use data for card
    data() {
        return {
            cardInfo: [
                {
                    title: "Donec English Action Movie",
                    category: "Coming Soon",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "505 Views",
                    src: this.getImagePath("2-1 (1).jpg")
                },
                {
                    title: "English Action Movie In Strack",
                    category: "Latest Movie",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "288 Views",
                    src: this.getImagePath("4-1.jpg")
                },
                {
                    title: "Movie Auctor Quisque In Strack",
                    category: "Top Rating",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "312 Views",
                    src: this.getImagePath("6.jpg")
                },
                {
                    title: "Auctor Movie Quisque In Strack",
                    category: "TV Series",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "362 Views",
                    src: this.getImagePath("5 (1).jpg")
                },
                {
                    title: "Donec Movie Quisque In Strack",
                    category: "Coming Soon",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "389 Views",
                    src: this.getImagePath("1-2.jpg")
                },
                {
                    title: "New Movie Quisque In Strack",
                    category: "Latest Movie",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "523 Views",
                    src: this.getImagePath("2.jpg")
                },
                {
                    title: "Quisque In Strack New Movie",
                    category: "Top Rating",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "372 Views",
                    src: this.getImagePath("3 (1).jpg")
                },
                {
                    title: "Nulla Strack New Animate Movie",
                    category: "TV Series",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "356 Views",
                    src: this.getImagePath("4.jpg")
                },
                {
                    title: "Blue Strack New Animate Movie",
                    category: "Coming Soon",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "442 Views",
                    src: this.getImagePath("3.jpg")
                },
                {
                    title: "Animate Blue Strack New Movie",
                    category: "Latest Movie",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "384 Views",
                    src: this.getImagePath("5 (1).jpg")
                },
                {
                    title: "Hurry Animate Blue Strack New Movie",
                    category: "Top Rating",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "476 Views",
                    src: this.getImagePath("1.jpg")
                },
                {
                    title: "Quisque Auctor Movie In Strack",
                    category: "Coming Soon",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "1069 Views",
                    src: this.getImagePath("2.jpg")
                },
                {
                    title: "New Movie Quisque In Strack",
                    category: "Latest Movie",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "774 Views",
                    src: this.getImagePath("5.jpg")
                },
                {
                    title: "Movie Action Garila English",
                    category: "Top Rating",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "388 Views",
                    src: this.getImagePath("3.jpg")
                },
                {
                    title: "Action Garila English Movie",
                    category: "TV Series",
                    release: "February 12, 2016",
                    genres: "Drama, Action Releas",
                    views: "313 Views",
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
            <h2 class="mt-4 ms-4"><b>Movie Playlist</b></h2>
            <p class="ms-4">Lorem Ipsum is simply dummy text of the printing and typesettin</p>
        </div>
        <div class="row">
            <div class="col-8">
                <!-- Use iframe to import Youtube Video -->
                <iframe class="mt-50" width="600" height="420"
                    src="https://www.youtube.com/embed/tgbNymZ7vqY?autoplay=1&mute=1">
                </iframe>
            </div>
            <div class="col-4 mt-50 bg-gray overflow-auto" style="height: 420px;">
                <h6 class="my-10"><b>New Movie</b></h6>
                <p class="fs-12">Plying 24</p>
                <hr>
                <!-- Use cycle to import img and text -->
                <div v-for="carte in cardInfo" class="row my-10">
                    <div class="col-4"><img :src="carte.src"></div>
                    <div class="col-8">
                        <h6><b>{{ carte.title }}</b></h6>
                        <div class="fs-12"><b>{{ carte.views }}</b></div>
                        <div class="d-flex justify-content-between">
                            <span class="fs-12">{{ carte.release }}</span>
                            <span class="fs-12">2.30.00</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>


    </section>
</template>

<style scoped>
.margin {
    margin: 100px 0;
}

.mt-50 {
    margin-top: 50px;
}

.my-10 {
    margin: 10px 0;
}

.fs-12 {
    font-size: 12px;
}

img {
    width: 100%;
    height: 100%;
}

.bg-gray {
    background-color: rgb(24, 32, 40);
}

.bg-gray::-webkit-scrollbar {
    width: 4px;
}

.bg-gray::-webkit-scrollbar-track {
    background-color: lightgrey;
    border-radius: 100px;
}

.bg-gray::-webkit-scrollbar-thumb {
    background-color: gray;
    border-radius: 100px;
}
</style>
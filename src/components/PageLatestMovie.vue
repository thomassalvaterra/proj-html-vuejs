<script>
export default {
    name: "PageLatestMovie",

    data() {
        return {
            cardInfo: [
                {
                    title: "Consequat Nam Lectus Nibh Aucibus It Has Turpis",
                    details: "Details",
                    share: "Share",
                    src: this.getImagePath("blog2.jpg")
                },
                {
                    title: "Nam Lectus Nibh Aucibus It Has Turpis",
                    details: "Details",
                    share: "Share",
                    src: this.getImagePath("blog3.jpg")
                },
                {
                    title: "Bring Me The Head Of Alfredo Garcia Best Movie In",
                    details: "Details",
                    share: "Share",
                    src: this.getImagePath("blog4-570x570.jpg")
                },
                {
                    title: "Pump Action Interaction English Action Movie (2020)",
                    details: "Details",
                    share: "Share",
                    src: this.getImagePath("blog5-570x570.jpg")
                }

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
            <h2 class="mt-4 ms-4"><b>Latest Movie</b></h2>
            <p class="ms-4">Lorem Ipsum is simply dummy text of the printing and typesettin</p>
        </div>
        <div class="row">
            <div class="col-6 position-relative">
                <img class="teschio mt-4" src="../assets/blog.jpg" alt="">
                <div class="position-absolute btm-20">
                    <h5 class="ml-10"><b>Actor The Concept Movie High Concept Theory See The Post</b></h5>
                    <hr>
                    <div class="d-flex justify-content-between align-items-center">
                        <div class="bg-col"><a href="#">Details</a></div>
                        <div class="mr-10">
                            <span class="mr-5"><a href="#">movistar</a></span>
                            <span class="mr-5"><a href="#">0 Comment</a></span>
                            <span class="mr-5"><a href="#">Share</a></span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-6 box mt-4 d-flex">
                <div class="row d-flex justiy-content-center align-items-center ml-10">
                    <div class="col-6 position-relative mb-3" v-for="carte in cardInfo">
                        <img :src="carte.src" class="hunter">
                        <div class="position-absolute bottom-0">
                            <h6 class="text-center p-10"><b>{{ carte.title }}</b></h6>
                            <div class="d-flex justify-content-between align-items-center">
                                <div class="bg-col"><a href="#">{{ carte.details }}</a></div>
                                <div class="mr-10"><a href="#">{{ carte.share }}</a></div>
                            </div>
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

.teschio {
    width: 480px;
    height: 415px;
    object-fit: cover;
    background-color: black;
    opacity: 0.2;
}

.hunter {
    width: 100%;
    height: 200px;
    object-fit: cover;
    background-color: black;
    opacity: 0.2;
}

.box {
    width: calc(100% / 2);
}

.img-bg {
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

.ml-10 {
    margin-left: 10px;
}

.p-10 {
    padding: 10px;
}

.mr-10 {
    margin-right: 15px;
}

.mr-5 {
    margin-right: 20px;
    font-size: 12px;
}

.mb-5 {
    margin-bottom: 3px;
}

.btm-20 {
    bottom: 30px;
}

a {
    text-decoration: none;
    color: white;
}
</style>
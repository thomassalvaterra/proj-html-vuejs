<!-- <script>
export default {
    name: "PageFooter",

    // props: {
    //     links: Object
    // }
}
</script>

<template>
     <div class="row">
        <div v-for="link in this.footerLinks" class="col-3">
            <h5>{{ links.title[0].type }}</h5>
            <p>{{ links.link[0].type }}</p>
        </div>
        <div class="col-3">
            <h5>{{ links.title[1].type }}</h5>
            <p>{{ links.link[1].type }}</p> -->
        <!-- </div>
        <div class="col-3">

        </div>
    </div> -->

<!-- </template>

<style scoped>
img {
    width: 100%;
    height: 450px;
    object-fit: cover;
}
</style> -->

<script>
export default {
    name: "PageFooter",
    data() {
        return {
            footerLinks: [
                {
                    title: "Movie Category",
                    link: ["English New Movie", "Hindi All Movie", "Latest Tamil Movie", "New Top Rating Movie", "Hornn New Movie", "Animation New Movie"]
                },
                {
                    title: "Information",
                    link: ["Youtube Video Post", "Actor Information", "New Promotion", "Latest Movie In English", "Latest Flim Product", "Video New Video"]
                },

            ],
            cardInfo: [
                {
                    title: "Actor The Concept High Concept Theory see",
                    release: "April 14, 2020",
                    src: this.getImagePath("5.jpg")
                },
                {
                    title: "consequat Nam lectus nibh aucibus It has turpis",
                    release: "April 14, 2020",
                    src: this.getImagePath("3.jpg")
                },
                {
                    title: "Nam lectus nibh consequat aucibus turpis",
                    release: "April 14, 2020",
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
    <div class="row mt-50">
        <div class="col-3">
            <h6><b>About Us</b></h6>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Exercitationem laboriosam error magni amet,
                sed
                doloremque fugit vero repellendus nulla corporis ipsum neque. Dolorem corporis necessitatibus cum
                pariatur
                sapiente est dolore?
            </p>
            <span class="ml"><a href="#"><i class="fa-brands fa-facebook lock fb mr-10"></i></a><a href="#"><i
                        class="fa-brands fa-twitter mr-10 lock tw"></i></a><a href="#"><i
                        class="fa-brands fa-linkedin mr-10 lock lk"></i></a><a href="#"><i
                        class="fa-brands fa-instagram mr-10 lock ig"></i></a><a href="#"><i
                        class="fa-brands fa-google-plus-g mr-10 lock gp"></i></a>
            </span>
        </div>
        <div class="col-6 d-flex justify-content-between">
            <div v-for="link in footerLinks">
                <h6><b>{{ link.title }}</b></h6>
                <div v-for="element in link.link"><a href="#">{{ element }}</a></div>
            </div>
        </div>
        <div class="col-3">
            <h6><b>Recent Posts</b></h6>
            <div v-for="carte in cardInfo" class="row my-10">
                <div class="col-4"><img :src="carte.src"></div>
                <div class="col-8">
                    <div class="fs-12"><b><a href="#">{{ carte.title }}</a></b></div>
                    <div class="fs-12">{{ carte.release }}</div>
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
.fb {
    color: blue;
}

.tw {
    color: lightskyblue;
}

.lk {
    color: aqua;
}

.ig {
    color: red;
}

.gp {
    color: orangered;
}

.fb:hover,
.tw:hover,
.lk:hover,
.ig:hover,
.gp:hover {
    color: rgb(19, 190, 19);
}

.mt-50 {
    margin-top: 50px;
}

img {
    width: 80px;
    height: 80px;
}

a {
    text-decoration: none;
    color: white;
}

a:hover {
    color: rgb(19, 190, 19);
}

.mr-10 {
    margin-right: 10px;
}

.fs-12 {
    font-size: 12px;
}
</style>
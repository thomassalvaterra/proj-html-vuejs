<script>
export default {
    name: "PageFooter",

    props: {
        links: Object
    }
}
</script>

<template>
    <div class="row">
        <div v-for="link in this.footerLinks" class="col-3">
            <h5>{{ links.title[0].type }}</h5>
            <p>{{ links.link[0].type }}</p>
        </div>
        <div class="col-3">
            <!-- <h5>{{ links.title[1].type }}</h5>
            <p>{{ links.link[1].type }}</p> -->
        </div>
        <div class="col-3">

        </div>
    </div>
</template>

<style scoped>
img {
    width: 100%;
    height: 450px;
    object-fit: cover;
}
</style>
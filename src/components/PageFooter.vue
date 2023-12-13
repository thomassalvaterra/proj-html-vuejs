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
        <div class="col-3">
            <p>{{ links.title }}</p>
            <p>{{ links.link.type }}</p>
        </div>
        <div class="col-3">
            {{ links.title }}
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
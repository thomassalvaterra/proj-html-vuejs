<script>
export default {
    name: "PageCountdown"
}
</script>

<template>
    <div class="position-relative z-n1">
        <img src="../assets/coming-bg.jpg">
    </div>
    <div class="d-flex justify-content-center ">
        <div class="w-25 text-center position-absolute top-50 left-50 z-0">
            <h6 class="cl-green"><b>COMING SOON MOVIE</b></h6>
            <h1 id="fs-50">MAX STILL</h1>
            <h3>JON PLAYER <span class="cl-green">&</span> EMILY ROSE</h3>

        </div>
    </div>
</template>

<style scoped>
img {
    width: 100%;
    height: 100%;
}

#fs-50 {
    font-size: 50px;
}

.cl-green {
    color: rgb(19, 190, 19);
}
</style>
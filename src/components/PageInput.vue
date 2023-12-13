<script>
export default {
    name: "PageInput"
}
</script>
<template>
    <section class="margin">
        <div class="position-relative">
            <img class="img-input" src="../assets/form-bg-1.png" alt="">
            <div class="row position-absolute btm-20">
                <div class="col-4">
                    <input class="form-control bg-green" type="text" placeholder="First Name"
                        aria-label="default input example">
                </div>
                <div class="col-4">
                    <input class="form-control bg-green" type="text" placeholder="Last Name"
                        aria-label="default input example">
                </div>
                <div class="col-4">
                    <input class="form-control bg-green" type="text" placeholder="Email Address"
                        aria-label="default input example">
                </div>
            </div>
            <div class="row position-absolute btm-15">
                <div class="col-12">
                    <button class="bte"><b>Subscribe</b></button>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
.margin {
    margin: 100px 0;
}

.img-input {
    width: 100%;
}

.btm-20 {
    bottom: 180px;
    left: 150px;
}

.btm-15 {
    bottom: 80px;
    left: 440px;
}

.bte {
    background-color: rgb(6, 15, 25);
    border: 1px solid rgb(6, 15, 25);
    border-radius: 30px;
    padding: 20px;
    color: white;
}

.bte:hover {
    background-color: white;
    color: black;
}

.bg-green {
    background-color: rgb(19, 190, 19);
    color: white;
}
</style>
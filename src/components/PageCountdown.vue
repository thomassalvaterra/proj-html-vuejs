<script>
export default {
    name: "PageCountdown",

    data() {
        return {
            countdown: '',
            countDownDate: new Date("dec 25, 2023 15:37:25").getTime(),
        };
    },
    mounted() {
        this.updateCountdown();
        this.timerInterval = setInterval(this.updateCountdown, 1000);
    },
    beforeDestroy() {
        clearInterval(this.timerInterval);
    },
    methods: {
        updateCountdown() {
            const now = new Date().getTime();
            const distance = this.countDownDate - now;
            if (distance >= 0) {
                const days = Math.floor(distance / (1000 * 60 * 60 * 24));
                const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
                const seconds = Math.floor((distance % (1000 * 60)) / 1000);
                this.countdown = `${days}d ${hours}h ${minutes}m ${seconds}s`;
            } else {
                clearInterval(this.timerInterval);
                this.countdown = "EXPIRED";
            }
        },
    },
}
</script>

<template>
    <div class="d-flex justify-content-center bg-img">
        <div class="w-25 text-center mt-info">
            <h6 class="cl-green"><b>COMING SOON MOVIE</b></h6>
            <h1 id="fs-50">MAX STILL</h1>
            <h3>JON PLAYER <span class="cl-green">&</span> EMILY ROSE</h3>
            <p>{{ this.countdown }}</p>
        </div>
    </div>
</template>

<style scoped>
.bg-img {
    background-image: url(../assets/coming-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    height: 600px;
}

#fs-50 {
    font-size: 50px;
}

.cl-green {
    color: rgb(19, 190, 19);
}

.mt-info {
    margin: 200px 0 0 450px;
}

p {
    text-align: center;
    font-size: 1.5rem;
}
</style>


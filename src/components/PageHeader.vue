<script>
export default {
  name: "PageHeader"
}
</script>

<template>
  <header>
    <div>
      <span><i class="fa-regular fa-envelope"></i>Superhit Top Movie<i class="fa-solid fa-star fs colgroup"></i><i
          class="fa-solid fa-star fs colgroup"></i><span class="colgroup">King Star</span><i
          class="fa-solid fa-star fs colgroup"></i><i class="fa-solid fa-star fs colgroup"></i></span>
      <span class="ml"><a href="#"><i class="fa-brands fa-facebook m-star"></i></a><a href="#"><i
            class="fa-brands fa-twitter m-star"></i></a><a href="#"><i class="fa-brands fa-linkedin m-star"></i></a><a
          href="#"><i class="fa-brands fa-instagram m-star"></i></a><a href="#"><i
            class="fa-brands fa-google-plus-g m-star"></i></a></span>
    </div>
    <div>
      <a href="#" class="lock"><i class="fa-solid fa-lock m-star"></i>Login</a>
    </div>
  </header>
  <hr>
  <section>
    <img src="/img/cropped - logo.png" alt="">
  </section>
</template>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 50px;
}

.fs {
  font-size: 7px;
}

.colgroup {
  color: rgb(19, 190, 19);
}

.ml {
  margin-left: 20px;
}

.m-star {
  margin: 5px;
}

.lock {
  color: white;
  text-decoration: none;
}
</style>

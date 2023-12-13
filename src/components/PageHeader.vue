<script>
export default {
  name: "PageHeader",

}
</script>

<template>
  <header>
    <div>
      <span><i class="fa-regular fa-envelope"></i>Superhit Top Movie<i class="fa-solid fa-star fs colgroup"></i><i
          class="fa-solid fa-star fs colgroup"></i><span class="colgroup">King Star</span><i
          class="fa-solid fa-star fs colgroup"></i><i class="fa-solid fa-star fs colgroup"></i></span>
      <span class="ml"><a href="#"><i class="fa-brands fa-facebook m-star lock fb"></i></a><a href="#"><i
            class="fa-brands fa-twitter m-star lock tw"></i></a><a href="#"><i
            class="fa-brands fa-linkedin m-star lock lk"></i></a><a href="#"><i
            class="fa-brands fa-instagram m-star lock ig"></i></a><a href="#"><i
            class="fa-brands fa-google-plus-g m-star lock gp"></i></a></span>
    </div>
    <div>
      <a href="#" class="lock"><i class="fa-solid fa-lock m-star"></i>Login</a>
    </div>
  </header>
  <hr>
  <section>
    <img src="../assets/cropped-logo.png" alt="Logo">
    <div class="input-group mb-3 w-50">
      <button class="btn btn-outline-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown"
        aria-expanded="false">All Movie</button>
      <ul class="dropdown-menu">
        <li><a class="dropdown-item" href="#">All Movie Category</a></li>
        <li><a class="dropdown-item" href="#">Coming Soon</a></li>
        <li><a class="dropdown-item" href="#">Latest Movie</a></li>
        <li><a class="dropdown-item" href="#">Top Rating</a></li>
        <li><a class="dropdown-item" href="#">TV Series</a></li>
      </ul>
      <input type="text" class="form-control bg-cl" placeholder="Search..." aria-label="Text input with dropdown button">
      <button class="btn bg-green">Search</button>
    </div>
  </section>
  <hr>
  <section>
    <nav class="navbar navbar-expand-lg ">
      <div class="container-fluid">
        <div class="collapse navbar-collapse" id="navbarNavDarkDropdown">
          <ul class="navbar-nav">
            <li class="nav-item dropdown">
              <button class="btn text-white dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">
                Home
              </button>
              <ul class="dropdown-menu dropdown-menu-dark">
                <li><a class="dropdown-item" href="#">Home</a></li>
                <li><a class="dropdown-item" href="#">Home 2</a></li>
                <li><a class="dropdown-item" href="#">Home 3</a></li>
                <li><a class="dropdown-item" href="#">Home 4</a></li>
                <li><a class="dropdown-item" href="#">Home 5</a></li>
                <li><a class="dropdown-item" href="#">Home 6</a></li>
              </ul>
            </li>
            <li class="nav-item dropdown">
              <button class="btn text-white dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">
                Celebrity
              </button>
              <ul class="dropdown-menu dropdown-menu-dark">
                <li><a class="dropdown-item" href="#">Celebrity</a></li>
                <li><a class="dropdown-item" href="#">Celebrity Single</a></li>
              </ul>
            </li>
            <li class="nav-item dropdown">
              <button class="btn text-white dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">
                Movie
              </button>
              <ul class="dropdown-menu dropdown-menu-dark">
                <li><a class="dropdown-item" href="#">Movie Post</a></li>
                <li><a class="dropdown-item" href="#">Top Rate Movie</a></li>
                <li><a class="dropdown-item" href="#">Movie Category</a></li>
                <li><a class="dropdown-item" href="#">Single Movie</a></li>
              </ul>
            </li>
            <li class="nav-item dropdown">
              <button class="btn text-white dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">
                Page
              </button>
              <ul class="dropdown-menu dropdown-menu-dark">
                <li><a class="dropdown-item" href="#">Pricing Table</a></li>
                <li><a class="dropdown-item" href="#">Call To Action</a></li>
                <li><a class="dropdown-item" href="#">My account</a></li>
                <li><a class="dropdown-item" href="#">Cart</a></li>
                <li><a class="dropdown-item" href="#">Checkout</a></li>
                <li><a class="dropdown-item" href="#">Wishlist</a></li>
              </ul>
            </li>
            <li class="nav-item dropdown">
              <button class="btn text-white dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">
                Shop
              </button>
              <ul class="dropdown-menu dropdown-menu-dark">
                <li>
                  <div class="btn-group dropend">
                    <button type="button" class="btn text-white dropdown-toggle" data-bs-toggle="dropdown"
                      aria-expanded="false">
                      Shop Sidebar
                    </button>
                    <ul class="dropdown-menu">
                      <li><a href="dropdown-item">Grid View</a></li>
                      <li><a href="dropdown-item">List View</a></li>
                    </ul>
                  </div>
                </li>
                <li>
                  <div class="btn-group dropend">
                    <button type="button" class="btn text-white dropdown-toggle" data-bs-toggle="dropdown"
                      aria-expanded="false">
                      No Sidebar
                    </button>
                    <ul class="dropdown-menu">
                      <li><a href="dropdown-item">Grid View</a></li>
                      <li><a href="dropdown-item">List View</a></li>
                    </ul>
                  </div>
                </li>
              </ul>
            </li>
            <li class="nav-item">
              <button class="btn text-white">
                Blog
              </button>
            </li>
            <li class="nav-item">
              <button class="btn text-white">
                Contact us
              </button>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <a href="#"><i class="fa-solid fa-basket-shopping lock"></i></a>
  </section>
</template>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 50px;
}

section {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 90px;
}

.fs {
  font-size: 7px;
}

.bg-cl {
  background-color: rgb(6, 15, 25);
}

.colgroup {
  color: rgb(19, 190, 19);
}

.bg-green {
  background-color: rgb(19, 190, 19);
  color: white;
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

a:hover {
  color: rgb(19, 190, 19);
}

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

button:hover {
  color: rgb(19, 190, 19);
}
</style>

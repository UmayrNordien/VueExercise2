<template>
  <nav class="navbar navbar-expand-lg bg-darker">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">sesh store</a>
      <a class="navbar-brand" href="#">
        <img
          src="https://i.postimg.cc/wMV5wg59/giphy-gif-cid-ecf05e47e0r9ohzqqhyozewkd7rt7zhdsskak98ypvphmn2e-rid-giphy.gif"
          width="100px" height="100px" alt="logo" class="logo">
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0 gap-2">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#"> <router-link to="/">Home</router-link></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><router-link to="/about">About</router-link></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><router-link to="/products">Products</router-link></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><router-link to="/contact">Contact</router-link></a>
          </li>
        </ul>
        <!-- <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form> -->
      </div>
    </div>
  </nav>
</template>

<script>
export default {

}
</script>
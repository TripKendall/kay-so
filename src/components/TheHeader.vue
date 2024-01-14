<template>
  <header class="main-header">
    <div class="container">
        <div class="container-fluid">
          <div class="logo d-flex align-items-center justify-content-between">
            <div class="container">
              <div class="row">
                <div class="col-12 col-md-auto">
                  <img src="/images/kay-so-header.webp" alt="Your Image" class="img-fluid">
                </div>
                <div class="col col d-flex align-items-center">
                  <h3>The Kay-So Podcast</h3>
                </div>
              </div>
            </div>
            <div>
              <a class="btn btn-primary" href="https://kay-so.com/rss.xml">
                Feed
              </a>
            </div>
          </div>
        </div>
    </div>
  </header>
</template>

<style scoped>
.main-header {
  background-color: #000;
  color: aliceblue;
  padding: 0 1rem;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 999;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.main-header .navbar {
  padding: 0;
}

.main-header .navbar .navbar-brand {
  padding: 0;
}

.main-header .navbar .navbar-brand img {
  width: 100px !important;
}



.main-header .navbar .navbar-collapse {
  padding: 0;
}

.main-header .navbar .navbar-collapse .navbar-nav {
  margin: 0;
}




</style>

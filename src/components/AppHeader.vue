<script>

export default {
  props: {
    navElements: Object,
  },

};
</script>
<template>
  <header>
    <div class="container">

      <!-- NAV -->
      <nav class="d-flex justify-content-between align-items-center mb-4">
        <!-- LOGO -->
        <a href="#">
          <img :src="navElements.src" alt="">
        </a>

        <ul class="d-flex align-items-center">
          <li><a href="#">{{ navElements.home }}</a></li>
          <li><a href="#">{{ navElements.about }}</a></li>
          <li><a href="#">{{ navElements.services }}</a></li>
          <li><a href="#">{{ navElements.blog }}</a></li>
          <li><a href="#">{{ navElements.contact }}</a></li>
          <li><a href="#">{{ navElements.portfolio }}</a></li>
          <li><a href="#" class="btn btn-primary">{{ navElements.sign }}</a></li>
        </ul>
      </nav>

    </div>

    <div class="container jumbotron">

      <!-- JUMBOTRON SX -->
      <div class="row">

        <div class="col-md-5 d-flex align-items-center">
          <div class="wrapper">

            <h1 class="text-start fw-bold">
              Business Planning <br>
              <span class="fw-normal">
                Digital Technology
              </span><br>
              Modern Solution!
            </h1>
            <p class="caption">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veritatis sit rem laudantium
              necessitatibus
              facilis officia accusantium at.</p>

            <a href="#" class="btn btn-danger me-3">Try it Now</a>
            <a href="#" class="btn btn-primary">Explore More</a>

          </div>
        </div>

        <!-- JUMBOTRON DX -->
        <div class="col-md-7">

          <!-- HERO IMAGE -->
          <div class="text-end">
            <img src="/images/header.png" alt="">
          </div>

        </div>
      </div>

    </div>
  </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/_variables.scss' as *;
@use '../styles/partials/_mixins.scss' as *;



header {
  padding: $small-size 0;
  background-color: rgb(99, 128, 206);
  color: white;
  @include bluegradient;

  nav li {
    margin: 0 $small-size;
  }

  .jumbotron {

    padding-bottom: $xxlarge-size;

    .wrapper {
      width: 350px;

      .caption {
        margin: $medium-size 0;
        color: #03A7D3E6;
      }
    }

    img {
      max-width: 600px;
      width: 100%;
    }
  }

}
</style>
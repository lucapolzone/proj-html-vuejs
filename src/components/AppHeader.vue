<script>
  
  export default {
    data() {
      return {

      }
    },

  };
</script>
<template>
  
  <header>
    <div class="container d-flex justify-content-between align-items-center mb-3">
      <!-- LOGO -->
      <a href="#">
        <img src="/images/white-logo-2.png" alt="">
      </a>
  
      <!-- NAV -->
      <nav>
        <ul class="d-flex align-items-center">
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Services</a></li>
          <li><a href="#">Blog</a></li>
          <li><a href="#">Contact</a></li>
          <li><a href="#">Portfolio</a></li>
          <li><a href="#" class="btn btn-primary">Sign in</a></li>
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
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veritatis sit rem laudantium necessitatibus facilis officia accusantium at.</p>

            <a href="#" class="btn btn-primary me-3">Try it Now</a>
            <a href="#" class="btn btn-primary">Explore More</a>

          </div>
        </div>

        <!-- JUMBOTRON DX -->
        <div class="col-md-7">
          
          <!-- HERO IMAGE -->
          <div class="text-center">
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
      margin: 0 $xsmall-size;
    }

    .jumbotron {

      padding-bottom: $xlarge-size;
      .wrapper {
        width: 350px;
      }

      img {
        height: 440px;
      }
    }

  }

  .debug {
    border-left: 2px solid green;
    border-right: 2px solid green;
  }



</style>
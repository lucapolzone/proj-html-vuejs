<script>
import AppCard from './AppCard.vue';


export default {
  data() {
    return {
      activeIndex: 0,
      

    }
  },

  methods: {
    changeIndex(newIndex) {
      this.activeIndex = newIndex;
    }


  },

  props: {
    cards: Array,
    slides: Array,
  },

  components: { AppCard }

};
</script>
<template>
  <main>

    <!-- SECTION OUR SERVICES -->
    <section id="our-services">
      <div class="container text-center">

        <div class="wrapper-title">
          <small>Our Services</small>
          <h2>What We Do</h2>
          <p>When, while the lovely valley teems with vapour around meand the</p>


        </div>

        <div class="row text-center">

          <app-card v-for="card in cards" :card="card" />

        </div>

        <a href="#" class="btn btn-danger me-3">View All Services</a>
      </div>
    </section>

    <!-- SECTION START YOUR PROJECT -->
    <section id="start-your-project">
      <div class="container">

        <!-- SX -->
        <div class="row d-flex align-items-center">

          <div class="col-md-5">

            <!-- IMAGE -->
            <div class="position-relative">
              <img class="men-data" src="/images/men-data.png" alt="">
              <img class="nemoodar" src="/images/nemoodar.png" alt="">
            </div>
          </div>

          <!-- DX -->
          <div class="col-md-6 d-flex justify-content-end">

            <div class="wrapper">

              <small>Start Your Project</small>
              <h2 class="text-start mt-4">
                Grow Your Business <br>
                <span class="fw-normal">
                  With Our Strategy
                </span>
              </h2>
              <p class="caption">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veritatis sit rem laudantium
                necessitatibus
                facilis officia accusantium at.</p>

              <a href="#" class="btn btn-danger me-3">Try it Now</a>
              <a href="#" class="btn btn-primary">Explore More</a>

            </div>


          </div>
        </div>

      </div>
    </section>

    <!-- SECTION PORTFOLIO -->
    <section id="portfolio">
      <div class="container">

        <div class="wrapper-top-content d-flex justify-content-between align-items-end">
          <div>
            <small>Portfolio</small>
            <h2>latest <span class="fw-normal">work</span></h2>
          </div>

          <div class="carousel-arrows">
            <i class="fa-solid fa-circle-arrow-left" ></i>
            <i class="fa-solid fa-circle-arrow-right"></i>
          </div>

        </div>

        <!-- ==== CAROUSEL ==== -->

        <div class="container carousel my-5">
          <div class="row">

            <div v-for="(slide, index) in slides" class="col">
              <div class="card ms-card">
                <div class="overlay-img-card">
                  <img :src="slide.imgPath" alt="">
                </div>
                <div class="badge-card d-flex align-items-center justify-content-around py-2">
                  <small class="fw-bold">
                    {{ slide.badge1 }}
                  </small>
                  <small>
                    {{ slide.badge2 }}
                  </small>
                </div>
              </div>
            </div>

          </div>

          <div class="text-center mt-3">
            <i class="fa-solid fa-circle"></i>
            <i class="fa-solid fa-circle"></i>
            <i class="fa-solid fa-circle active"></i>
            <i class="fa-solid fa-circle"></i>
            <i class="fa-solid fa-circle"></i>
          </div>
        </div>

      </div>
    </section>

    <section id="price-list" class="text-center">
      
      <div class="wrapper-title">
        <small>Price List</small>
        <h2>Our Pricing</h2>
        <p>When, while the lovely valley teems with vapour around meand the</p>
      </div>

      <div class="container my-5">
          <div class="row gx-4">
          <div class="col-md-4">

            <div class="card rounded-4 p-5">
              <h2>40</h2>

              <h2>Designing</h2>
              <small>PROCESS</small>
              <small class="mt-3 dollar-symbol">$</small>
              <h2>40</h2>
              <small>Per Month</small>

              <ul class="my-5">
                <li><small><span class="fw-bold">Creative </span>Designed Enabled</small></li>
                <li><small><span class="fw-bold">Vibrant </span>Color Usage</small></li>
                <li><small><span class="fw-bold">Eye </span>Catching Design</small></li>
                <li><small><span class="fw-bold">Extreme </span>Typography</small></li>
                <li><small><span class="fw-bold">Exceptional </span>Design</small></li>
              </ul>

              <div>
                <a href="#" class="btn btn-danger vertical">Order Now<i class="ms-5 fa-solid fa-arrow-right-long"></i></a>
              </div>


            </div>

          </div>
          <div class="col-md-4">
            
            <div class="card rounded-4 p-5">
              <h2>60</h2>

              <h2>Developing</h2>
              <small>PRODUCT</small>
              <small class="mt-3 dollar-symbol">$</small>
              <h2>60</h2>
              <small>Per Month</small>

              <ul class="my-5">
                <li><small><span class="fw-bold">Creative </span>Designed Enabled</small></li>
                <li><small><span class="fw-bold">Vibrant </span>Color Usage</small></li>
                <li><small><span class="fw-bold">Eye </span>Catching Design</small></li>
                <li><small><span class="fw-bold">Extreme </span>Typography</small></li>
                <li><small><span class="fw-bold">Exceptional </span>Design</small></li>
              </ul>

              <div>
                <a href="#" class="btn btn-outline-danger">Order Now<i class="ms-5 fa-solid fa-arrow-right-long"></i></a>
              </div>


            </div>

          </div>
          <div class="col-md-4">
            
            <div class="card rounded-4 p-5">
              <h2>80</h2>

              <h2>Supporting</h2>
              <small>CLIENTS</small>
              <small class="mt-3 dollar-symbol">$</small>
              <h2>80</h2>
              <small>Per Month</small>

              <ul class="my-5">
                <li><small><span class="fw-bold">Creative </span>Designed Enabled</small></li>
                <li><small><span class="fw-bold">Vibrant </span>Color Usage</small></li>
                <li><small><span class="fw-bold">Eye </span>Catching Design</small></li>
                <li><small><span class="fw-bold">Extreme </span>Typography</small></li>
                <li><small><span class="fw-bold">Exceptional </span>Design</small></li>
              </ul>

              <div>
                <a href="#" class="btn btn-danger vertical">Order Now<i class="ms-5 fa-solid fa-arrow-right-long"></i></a>
              </div>


            </div>

          </div>
        </div>
      </div>
    </section>


  </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/_variables.scss' as *;
@use '../styles/partials/_mixins.scss' as *;


main {

  section {
    padding: $large-size 0;
  }

  .wrapper-title {
    text-align: center;

    small {
      color: #F9636B;
    }
  }

  // section#our-services {
  // }

  section#start-your-project {

    .men-data {
      max-width: 400px;
      position: absolute;
      right: 0;
      bottom: 0;
    }

    .nemoodar {
      max-width: 500px;
      margin-bottom: 5rem;
    }


    .wrapper {
      width: 400px;

      .caption {
        @include caption
      }
    }

  }


  section#portfolio {


    .carousel-arrows {
      color: #F9636B;

      .fa-solid {
        font-size: $medium-size;
      }
      .fa-solid.fa-circle-arrow-left {
        margin-right: 1rem;
      }

    }

 
    .carousel {

      .ms-card {
        border-radius: 20px;

        .badge-card {
          font-size: $small-size;
        }

        .overlay-img-card {
          border-radius: 20px;
          overflow: hidden;

          img {
            object-fit: cover;
            height: 180px;
          }
        }

      }
    }

    .fa-solid.fa-circle {
      font-size: $xsmall-size;
      margin: 0 $xxsmall-size;
      color: #e0e0e0;

      &.active {
        color: #F9636B;
      }

    }

  }

  section#price-list {
    background-image: linear-gradient(to bottom, #0a1852 0, #01002f 50%, #fff 50%, #fff 100%);
    .card {
      position: relative;

      .dollar-symbol {
        margin-right: $xxlarge-size;
      }

      h2:first-of-type {
        font-size: 15rem;
        position: absolute;
        top: -75px;
        right: -10px;
        opacity: .1;
      }
      
      h2:last-of-type {
      font-size: $xxlarge-size;
      line-height: 4.2rem;
      }
    }

    .container .col-md-4:nth-of-type(even) .card {
      background-image: linear-gradient(to bottom, #B6246E 0, #F9636B 100%);
      color: white;
        .btn {
          background-color: #fff;
        }
    }
  }


}
</style>
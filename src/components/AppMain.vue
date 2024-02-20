<script>
import AppCard from './AppCard.vue';


export default {
  data() {
    return {

    }
  },

  props: {
    cards: Array,
  },

  components: { AppCard }

};
</script>
<template>
  <main>

    <!-- SECTION OUR SERVICES -->
    <section id="our-services">
      <div class="container text-center">

        <div class="wrapper-title text-center">
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

        <div class="wrapper-title">
          <small>Portfolio</small>
          <h2>latest <span class="fw-normal">work</span></h2>
        </div>

        <div class="container carousel">
          <div class="row">

            <div class="col-md-3">
              <div class="card ms-card">
                <div class="img-card" id="img1">
                </div>
                <div class="caption-card d-flex align-items-center justify-content-around py-2">
                  <small class="fw-bold">
                    Caption 1
                  </small>
                  <small>
                    Caption 2
                  </small>
                </div>
              </div>
            </div>

            <div class="col-md-3">
              <div class="card ms-card">
                <div class="img-card" id="img2">
                </div>
                <div class="caption-card d-flex align-items-center justify-content-around py-2">
                  <small class="fw-bold">
                    Caption 1
                  </small>
                  <small>
                    Caption 2
                  </small>
                </div>
              </div>
            </div>

            <div class="col-md-3">
              <div class="card ms-card">
                <div class="img-card" id="img3">
                </div>
                <div class="caption-card d-flex align-items-center justify-content-around py-2">
                  <small class="fw-bold">
                    Caption 1
                  </small>
                  <small>
                    Caption 2
                  </small>
                </div>
              </div>
            </div>

            <div class="col-md-3">
              <div class="card ms-card">
                <div class="img-card" id="img4">
                </div>
                <div class="caption-card d-flex align-items-center justify-content-around py-2">
                  <small class="fw-bold">
                    Caption 1
                  </small>
                  <small>
                    Caption 2
                  </small>
                </div>
              </div>
            </div>

          </div>

          <div class="text-center">
            <i class="fa-solid fa-circle active"></i>
            <i class="fa-solid fa-circle"></i>
            <i class="fa-solid fa-circle"></i>
            <i class="fa-solid fa-circle"></i>
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
    .carousel {
      // overflow-x: auto;
      border: 2px solid red;

      .ms-card {
        border-radius: 20px;

        .img-card {
          border-radius: 20px;
          height: 250px;
          background-size: cover;

          &#img1 {
            background-image: url('/images/84316050-0af0-49db-a53a-241d47ddad0e-2-790x576.jpg');
          }

          &#img2 {
            background-image: url('/images/a247b00b-3621-470f-b4b8-b3ac46f25907-1-790x576.jpg');
          }

          &#img3 {
            background-image: url('/images/8wa60okr-1-790x576.jpg');
          }

          &#img4 {
            background-image: url('/images/DRY-1-790x576.jpg');
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


}
</style>
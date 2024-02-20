<script>
import AppCard from './AppCard.vue';


export default {
  data() {
    return {
      index: 0,
      slides: [
        {
          imgPath: '/images/84316050-0af0-49db-a53a-241d47ddad0e-2-790x576.jpg',
          badge1: 'Mock-up',
          badge2: 'Digital Experience'
        },
        {
          imgPath: '/images/8wa60okr-1-790x576.jpg',
          badge1: 'Basket of Flower on table',
          badge2: 'Branding Strategy'
        },
        {
          imgPath: '/images/DRY-1-790x576.jpg',
          badge1: 'Purinky Products',
          badge2: 'Digital Experience'
        },
        {
          imgPath: '/images/a247b00b-3621-470f-b4b8-b3ac46f25907-1-790x576.jpg',
          badge1: 'Satisfy Poster',
          badge2: 'Branding Strategy'
        },
        {
          imgPath: '/images/studio-republic-644339-unsplash-1380x703.jpg',
          badge1: 'Office Poster',
          badge2: 'Team Work'
        }
      ]

    }
  },

  methods: {
    

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

        <div class="wrapper-top-content d-flex justify-content-between align-items-end">
          <div>
            <small>Portfolio</small>
            <h2>latest <span class="fw-normal">work</span></h2>
          </div>

          <div class="carousel-arrows">
            <i class="fa-solid fa-circle-arrow-left"></i>
            <i class="fa-solid fa-circle-arrow-right"></i>
          </div>

        </div>

        <!-- ==== CAROUSEL ==== -->

        <div class="container carousel">
          <div class="row">

            <div v-for="slide in slides" class="col">
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

          <div class="text-center">
            <i class="fa-solid fa-circle"></i>
            <i class="fa-solid fa-circle"></i>
            <i class="fa-solid fa-circle active"></i>
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
      // overflow-x: auto;
      border: 2px solid red;

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


}
</style>
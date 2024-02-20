<script>
import AppCard from './AppCard.vue';



export default {
  data() {
    return {

    }
  },

  components: { AppCard }

};
</script>
<template>
  <main>

    <section id="our-services">
      <div class="container text-center">

        <div class="wrapper-title">
          <small>Our Services</small>
          <h2>What We Do</h2>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
        </div>

        <div class="row text-center">

          <div class="col-md-3">
            <app-card :imgPath="'/images/Group-247.png'" :title="'Data Analysis'" />
          </div>

          <div class="col-md-3">
            <app-card :imgPath="'/images/Group-567.png'" :title="'SEO Optimization'" />
          </div>

          <div class="col-md-3">
            <app-card :imgPath="'/images/Group-538.png'" :title="'Security Data'" />
          </div>

          <div class="col-md-3">
            <app-card :imgPath="'/images/Group-566.png'" :title="'Branding Strategy'" />
          </div>

        </div>

        <a href="#" class="btn btn-danger me-3">View All Services</a>
      </div>
    </section>

    <section id="start-your-project">
      <div class="container">

        <!-- SX -->
        <div class="row  d-flex align-items-center">

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

}
</style>
<script>

export default {
  data() {
    return {

    }
  },

};
</script>
<template>
  <main>

    <section>
      <div class="container">
        SEZIONE BIANCA
      </div>
    </section>

    <section>
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
              <h1 class="text-start fw-bold mt-4">
                Grow Your Business <br>
                <span class="fw-normal">
                  With Our Strategy
                </span>
              </h1>
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


}

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
</style>
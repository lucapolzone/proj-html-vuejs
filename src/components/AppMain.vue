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
    <div class="container text-center">
      MAIN
    </div>

    <section>
      <div class="container">
        SEZIONE BIANCA
      </div>
    </section>

    <section id="blu">
      <div class="container">
        SEZIONE BLU
      </div>
    </section>


  </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/_variables.scss' as *;

main {


  section {
    padding: 7rem 0;
  }


}
</style>
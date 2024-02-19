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
    <div class="container d-flex justify-content-between align-items-center">
      <!-- LOGO -->
      <img src="/images/white-logo-2.png" alt="">
  
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
    
    <div class="container">
      <div class="jumbotron">
        JUMBOTRON
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

    nav li {
      margin: 0 $xsmall-size;
    }
  }



</style>
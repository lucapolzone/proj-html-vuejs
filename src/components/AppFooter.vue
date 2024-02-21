<script>

export default {
  data() {
    return {

    }
  },

};
</script>
<template>
  <footer>
    <section>
      <div class="container">
        <div class="row">

          <div class="col ms_align">
            <div class="card">
              <ul>
                <li>
                  <img src="/images/white-logo-2.png" alt="">
                </li>
              </ul>
              <div class="caption">
                <p>
                  When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper
                </p>
              </div>
            </div>
          </div>

          <div class="col ms_align">
            <div class="card">
              <h5>Quick Links</h5>
              <div class="caption">
                <p>Services</p>
                <p>Contact</p>
                <p>Blog</p>
              </div>
            </div>
          </div>

          <div class="col ms_align">
            <div class="card">
              <h5>Resources</h5>
              <div class="caption">
                <p>Art Design</p>
                <p>Computer</p>
                <p>IT News</p>
                <p>Networking</p>
                <p>Web Security</p>
              </div>
            </div>
          </div>

          <div class="col ms_align">
            <div class="card">
              <h5>Contact Us</h5>
              <div class="caption">
                <p><span>Address: </span>Patricia C. Amedee 4401 Waldeck Street Grapevine Nashville, Tx 76051</p>
                <p><span>Phone: </span>+99 (0) 101 0000 888</p>
                <p><span>Email: </span>Info©yourdomain.com</p>
              </div>
            </div>
          </div>

        </div>
      </div>
    </section>


  </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/_variables.scss' as *;
@use '../styles/partials/_mixins.scss' as *;


footer {
  @include bluegradient;
  padding: $xlarge-size 0;

  section {
    border-bottom: 1px solid rgba(129, 130, 154, 0.5);

    .card {
      background-color: transparent;
      border-radius: 0;
      color: white;
      border: none;

      img {
        width: auto;
      }

      .caption {
        color: #81829a;

        span {
          color: white;
        }
      }
    }
  }

  .ms_align {
    display: flex;
    justify-content: center;
  }

  .col:last-of-type {
    min-width: 370px;
  }

}
</style>
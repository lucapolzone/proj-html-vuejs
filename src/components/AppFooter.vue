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
    <div id="top-section" class="py-5">
      <div class="container">
        <div class="row">

          <div class="col ms_align">
            <div class="card">
              <ul>
                <li class="mb-3">
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
                <a href="#">
                  <p>Services</p>
                </a>
                <a href="#">
                  <p>Contact</p>
                </a>
                <a href="#">
                  <p>Blog</p>
                </a>
              </div>
            </div>
          </div>

          <div class="col ms_align">
            <div class="card">
              <h5>Resources</h5>
              <div class="caption">
                <a href="#">
                  <p>Art Design</p>
                </a>
                <a href="#">
                  <p>Computer</p>
                </a>
                <a href="#">
                  <p>IT News</p>
                </a>
                <a href="#">
                  <p>Networking</p>
                </a>
                <a href="#">
                  <p>Web Security</p>
                </a>
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
    </div>

    <div id="bottom-section" class="py-4">
      <div class="container d-flex justify-content-between">
        <p class="caption">© 2020 Phlox. All Rights Reserved</p>

        <ul class="d-flex">
          <li>
            <a href="#">
              <i class="fa-brands fa-instagram"></i>
            </a>
          </li>
          <li>
            <a href="#">
              <i class="fa-brands fa-linkedin-in"></i>
            </a>
          </li>
          <li>
            <a href="#">
              <i class="fa-brands fa-facebook-f"></i>
            </a>
          </li>
          <li>
            <a href="#">
              <i class="fa-brands fa-twitter"></i>
            </a>
          </li>
        </ul>
      </div>

    </div>


  </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/_variables.scss' as *;
@use '../styles/partials/_mixins.scss' as *;


.caption {
  color: #81829a;

  a {
    color: #81829a;

    &:hover {
      color: #F9636B;
    }
  }
}

footer {
  @include bluegradient;
  // padding: $xlarge-size 0;

  #top-section {
    border-bottom: 1px solid rgba(129, 130, 154, 0.5);

    .card {
      background-color: transparent;
      border-radius: 0;
      color: white;
      border: none;
      // border: 2px solid green;


      img {
        width: auto;
      }


      span {
        color: white;
      }
    }

    .ms_align {
      display: flex;
      justify-content: center;
      // border: 2px solid red;
    }


    .col:nth-of-type(2) {
      padding-left: $medium-size;
    }

    .col:nth-of-type(3) {
      padding-right: $xlarge-size;
    }

    .col:last-of-type {
      // flex-grow: 0;
      min-width: 370px;
    }

  }

  #bottom-section {

    li {
      margin: 0 $small-size;
    }
  }

}
</style>
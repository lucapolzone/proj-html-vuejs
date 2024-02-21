<script>
export default {
  props: {
    companyCard: Object,
    quickLinks: Object,
    resources: Object,
    contactUs: Object,
    copyright: String,
    socials: Object
  }

}
</script>
<template>
  <footer>
    <div id="widget" class="d-flex justify-content-between p-3">
      <div>
        <a href="#header">
          <i class="fa-solid fa-circle-arrow-up"></i>
        </a>
      </div>
      <div>
        <i class="fa-solid fa-comment-dots"></i>
      </div>
    </div>

    <div id="top-section" class="pb-5">
      <div class="container">
        <div class="row">

          <div class="col ms_align">
            <div class="card">
              <ul>
                <li class="mb-3">
                  <img :src="companyCard.imgPath" alt="">
                </li>
              </ul>
              <div class="caption">
                <p>
                  {{ companyCard.caption }}
                </p>
              </div>
            </div>
          </div>

          <div class="col ms_align">
            <div class="card">
              <h5>Quick Links</h5>
              <div class="caption">
                <a href="#">
                  <p>
                    {{ quickLinks.link1 }}
                  </p>
                </a>
                <a href="#">
                  <p>
                    {{ quickLinks.link2 }}
                  </p>
                </a>
                <a href="#">
                  <p>
                    {{ quickLinks.link3 }}
                  </p>
                </a>
              </div>
            </div>
          </div>

          <div class="col ms_align">
            <div class="card">
              <h5>Resources</h5>
              <div class="caption">
                <a href="#">
                  <p>
                    {{ resources.link1 }}
                  </p>
                </a>
                <a href="#">
                  <p>
                    {{ resources.link2 }}
                  </p>
                </a>
                <a href="#">
                  <p>
                    {{ resources.link3 }}
                  </p>
                </a>
                <a href="#">
                  <p>
                    {{ resources.link4 }}
                  </p>
                </a>
                <a href="#">
                  <p>
                    {{ resources.link5 }}
                  </p>
                </a>
              </div>
            </div>
          </div>

          <div class="col ms_align">
            <div class="card">
              <h5>Contact Us</h5>
              <div class="caption">
                <p><span>Address: </span>
                  {{ contactUs.address }}
                </p>
                <p><span>Phone: </span>
                  {{ contactUs.phone }}
                </p>
                <p><span>Email: </span>
                  {{ contactUs.email }}
                </p>
              </div>
            </div>
          </div>

        </div>
      </div>
    </div>

    <div id="bottom-section" class="py-4">
      <div class="container d-flex justify-content-between">
        <p class="caption">
          {{ copyright }}
        </p>

        <ul class="d-flex">
          <li>
            <a href="#">
              <i :class="socials.instagram"></i>
            </a>
          </li>
          <li>
            <a href="#">
              <i :class="socials.linkedin"></i>
            </a>
          </li>
          <li>
            <a href="#">
              <i :class="socials.facebook"></i>
            </a>
          </li>
          <li>
            <a href="#">
              <i :class="socials.twitter"></i>
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
  padding-top: 10rem;
  position: relative;

  #widget {
    position: absolute;
    bottom: 0;
    right: 0;
    width: 120px;
    font-size: $medium-size;
  }

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
<script>
export default {
  props: {
    footerElements: Array
  }

}
</script>
<template>
  <footer>
    <div id="top-section" class="pb-5">
      <div class="container">
        <div class="row">

          <div class="col ms_align">
            <div class="card">
              <ul>
                <li class="mb-3">
                  <img :src="footerElements[0].companyCard.imgPath" alt="">
                </li>
              </ul>
              <div class="caption">
                <p>
                  {{ footerElements[0].companyCard.caption }}
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
                    {{ footerElements[1].quickLinks.link1 }}
                  </p>
                </a>
                <a href="#">
                  <p>
                    {{ footerElements[1].quickLinks.link2 }}
                  </p>
                </a>
                <a href="#">
                  <p>
                    {{ footerElements[1].quickLinks.link3 }}
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
                    {{ footerElements[2].resources.link1 }}
                  </p>
                </a>
                <a href="#">
                  <p>
                    {{ footerElements[2].resources.link2 }}
                  </p>
                </a>
                <a href="#">
                  <p>
                    {{ footerElements[2].resources.link3 }}
                  </p>
                </a>
                <a href="#">
                  <p>
                    {{ footerElements[2].resources.link4 }}
                  </p>
                </a>
                <a href="#">
                  <p>
                    {{ footerElements[2].resources.link5 }}
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
                  {{ footerElements[3].contactUs.address }}
                </p>
                <p><span>Phone: </span>
                  {{ footerElements[3].contactUs.phone }}
                </p>
                <p><span>Email: </span>
                  {{ footerElements[3].contactUs.email }}
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
          {{ footerElements[4].bottomSection.copyright }}
        </p>

        <ul class="d-flex">
          <li>
            <a href="#">
              <i :class="footerElements[4].bottomSection.socials[0].instagram"></i>
            </a>
          </li>
          <li>
            <a href="#">
              <i :class="footerElements[4].bottomSection.socials[0].linkedin"></i>
            </a>
          </li>
          <li>
            <a href="#">
              <i :class="footerElements[4].bottomSection.socials[0].facebook"></i>
            </a>
          </li>
          <li>
            <a href="#">
              <i :class="footerElements[4].bottomSection.socials[0].twitter"></i>
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
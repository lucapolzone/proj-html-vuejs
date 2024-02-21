<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  data() {
    return {
      navElements: {
        imgPath: '/images/white-logo-2.png',
        home: 'Home',
        about: 'About',
        services: 'Services',
        blog: 'Blog',
        contact: 'Contact',
        portfolio: 'Portfolio',
        sign: 'Sign in'
      },
      cards: [
        {
          imgPath: '/images/Group-247.png',
          title: 'Data Analysis',
          caption: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
        },
        {
          imgPath: '/images/Group-567.png',
          title: 'SEO Optimization',
          caption: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
        },
        {
          imgPath: '/images/Group-538.png',
          title: 'Security Data',
          caption: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
        },
        {
          imgPath: '/images/Group-566.png',
          title: 'Branding Strategy',
          caption: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
        }
      ],
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
      ],
      footerElements: [
        {
          companyCard: {
            imgPath: '/images/white-logo-2.png',
            caption: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
          }
        },
        {
          quickLinks: {
            link1: 'Services',
            link2: 'Contact',
            link3: 'Blog'
          }
        },
        {
          resources: {
            link1: 'Art Design',
            link2: 'Computer',
            link3: 'IT News',
            link4: 'Networking',
            link5: 'Web Security'
          }
        },
        {
          contactUs: {
            address: 'Patricia C. Amedee 4401 Waldeck Street Grapevine Nashville, Tx 76051',
            phone: '+99 (0) 101 0000 888',
            email: 'Info©yourdomain.com'
          }
        },
        {
          bottomSection: {
            copyright: '© 2020 Phlox. All Rights Reserved',
            socials: [
              {
                instagram: 'fa-brands fa-instagram',
                linkedin: 'fa-brands fa-linkedin-in',
                facebook: 'fa-brands fa-facebook-f',
                twitter: 'fa-brands fa-twitter',
              }
            ]
          }
        }
      ]
    }
  },

  components: { AppHeader, AppMain, AppFooter }

};

</script>

<template>
  <app-header :navElements="navElements" />
  <app-main :cards="cards" :slides="slides" />
  <app-footer :footerElements="footerElements" />
</template>

<style lang="scss">
@use './styles/general.scss';
@use './styles/partials/_variables.scss';
</style>


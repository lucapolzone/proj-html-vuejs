<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  data() {
    return {
      navElements: {
        src: '/images/white-logo-2.png',
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
      ]
    }
  },

  components: { AppHeader, AppMain, AppFooter }

};

</script>

<template>
  <app-header :navElements="navElements" />
  <app-main :cards="cards" :slides="slides" />
  <app-footer />
</template>

<style lang="scss">
@use './styles/general.scss';
@use './styles/partials/_variables.scss';
</style>


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
      ]
    }
  },

  components: { AppHeader, AppMain, AppFooter }

};

</script>

<template>
  <app-header :navElements="navElements" />
  <app-main :cards="cards" />
  <app-footer />
</template>

<style lang="scss">
@use './styles/general.scss';
@use './styles/partials/_variables.scss';
</style>


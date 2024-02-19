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
      }
    }
  },

  components: { AppHeader, AppMain, AppFooter }

};

</script>

<template>
  <app-header :navElements="navElements" />
  <app-main />
  <app-footer />
</template>

<style lang="scss">
@use './styles/general.scss';
@use './styles/partials/_variables.scss';
</style>


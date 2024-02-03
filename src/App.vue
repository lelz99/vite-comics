<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import FooterTop from './components/FooterTop.vue';
import FooterBottom from './components/FooterBottom.vue';

import {
  films,
  headerLinks,
  infoLinks,
  otherSitesLinks,
  socials,
  infoMain
} from './assets/data';

export default {
  name: 'MyApp',
  components: { AppHeader, AppMain, FooterTop, FooterBottom },
  data: () => ({
    films,
    headerLinks,
    infoLinks,
    otherSitesLinks,
    socials,
    infoMain,
  })
}
</script>

<template>
  <AppHeader :headerLinks="headerLinks" />
  <AppMain />
  <FooterTop :otherSitesLinks="otherSitesLinks" :listLinks="headerLinks" :infoLinks="infoLinks" />
  <FooterBottom :socials="socials" />
</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>

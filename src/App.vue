<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import {
  films,
  headerLinks,
  infoLinks,
  otherSitesLinks,
  social,
  infoMain
} from './assets/data';

export default {
  name: 'MyApp',
  components: { AppHeader, AppMain, AppFooter },
  data: () => ({
    films,
    headerLinks,
    infoLinks,
    otherSitesLinks,
    social,
    infoMain
  })
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>

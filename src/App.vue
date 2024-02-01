<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  name: 'MyApp',
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.border {
  border: 1px dashed black;
}

.container {
  max-width: 920px;
  margin: 0 auto;
}
</style>

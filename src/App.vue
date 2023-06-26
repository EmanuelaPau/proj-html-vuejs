<template>
  <div class="app">
    <AppHeader />
    <AppMain />
    <AppFooter />

  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  }
}
</script>
<style lang="scss">
@import './styles/general.scss';
@import './styles/partials/variables';
@import "bootstrap/scss/bootstrap";

div.app {
  font-family: 'Roboto', sans-serif;
  background-color: $colorSecondary;
  color: $colorLight;
}
</style>

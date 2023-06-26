<template>
  <div>
    <HelloWorld>
    </HelloWorld>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>
<style lang="scss">
@import './styles/general.scss';
@import "bootstrap/scss/bootstrap";
</style>

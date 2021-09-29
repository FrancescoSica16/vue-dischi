<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Main msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import Main from './components/Main.vue'

export default {
  name: 'App',
  components: {
    Main,
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import ".style/general.scss";


</style>

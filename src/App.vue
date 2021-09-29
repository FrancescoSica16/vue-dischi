<template>
  <div id="app">

    <MusicGroup/>

  </div>
</template>

<script>
import MusicGroup from './components/MusicGroup.vue'


export default {
  name: 'App',
  components: {
    MusicGroup,
  }
}
</script>

<style  lang="scss">
@import "style/general.scss";
@import "style/variabiles.scss";


</style>

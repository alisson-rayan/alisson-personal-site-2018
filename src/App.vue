<template>
  <div id="app">
    <landing-page-container />
  </div>
</template>

<script>
import LandingPageContainer from './containers/LandingPageContainer'

export default {
  name: 'app',
  components: {
    LandingPageContainer
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
  padding: 0;
}
</style>

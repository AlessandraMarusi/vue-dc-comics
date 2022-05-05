<template>
  <div id="app">
    <app-header/>
    <main>
      <app-jumbotron/>
      <app-grid/>
      <app-icon-bar/>
    </main>
    <footer>
      <app-footer-top/>
      <app-footer-bottom/>
    </footer>
    
  </div>
</template>

<script>
import AppFooterBottom from './components/AppFooterBottom.vue'
import AppFooterTop from './components/AppFooterTop.vue'
import AppGrid from './components/AppGrid.vue'
import AppHeader from './components/AppHeader.vue'
import AppIconBar from './components/AppIconBar.vue'
import AppJumbotron from './components/AppJumbotron.vue'


export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooterTop,
    AppFooterBottom,
    AppIconBar,
    AppJumbotron,
    AppGrid

  }
}
</script>

<style lang="scss">
@import './style/generals';
@import './style/variables';
</style>

<template>
  <div id="app">
    <app-header/>
    <main>
      <app-content/>
      <app-icon-bar/>
    </main>
    <footer>
      <app-footer-top/>
      <app-footer-bottom/>
    </footer>
    
  </div>
</template>

<script>
import AppContent from './components/AppContent.vue'
import AppFooterBottom from './components/AppFooterBottom.vue'
import AppFooterTop from './components/AppFooterTop.vue'
import AppHeader from './components/AppHeader.vue'
import AppIconBar from './components/AppIconBar.vue'


export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooterTop,
    AppContent,
    AppFooterBottom,
    AppIconBar

  }
}
</script>

<style lang="scss">
@import './style/generals';
@import './style/variables';
</style>

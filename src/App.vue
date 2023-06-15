<template>
  <div>
    <AppHeader />
    <AppMainSelection />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'

import AppMainSelection from './components/AppMainSelection.vue'

import AppFooter from './components/AppFooter.vue'


export default {
  name: 'App',
  components: {
    AppHeader,
    AppMainSelection,
    AppFooter
  }
}
</script>
<style lang=“scss”>
  @import "./components/styles/general.scss"
</style>

<template>
  <div>
    <AppHeader />
    <AppMainSelection />
    <AppMainChoice />
    <AppFooter />

  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'

import AppMainSelection from './components/AppMainSelection.vue'

import AppMainChoice from './components/AppMainChoice.vue'

import AppFooter from './components/AppFooter.vue'



export default {
  name: 'App',
  components: {
    AppHeader,
    AppMainSelection,
    AppMainChoice,
    AppFooter
  }
}
</script>

<style lang="scss">
@import './styles/general.scss';

/* Google font  */
@import url('https://fonts.googleapis.com/css2?family=PT+Sans+Caption:wght@400;700&family=PT+Sans:ital,wght@0,400;0,700;1,400;1,700&display=swap');

div {
  font-family: 'PT Sans', sans-serif;
}
</style>


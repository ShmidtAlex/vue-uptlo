<template>
  <div id="app">
    
    <background></background>
    <app-header></app-header>
    
  </div>
</template>

<script>

import Header from './components/Header'
import Background from './components/Background'

export default {
  name: 'app',
  components: {
    'background':Background,
    'app-header':Header,

  }
}
</script>

<style lang="less">


</style>

<template>
  <div id="app">
    <fun-components></fun-components>
  </div>
</template>

<script>
import FunComponents from '@/components/FunComponent.vue'

export default {
  name: 'App',
  components: {
    FunComponents,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

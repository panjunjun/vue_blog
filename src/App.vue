<template>
  <div id="app">
    <app-header></app-header>
    <!-- <router-view/> -->
    <mario-animation></mario-animation>
    <app-footer></app-footer>
  </div>
</template>

<script>
import header from './components/header.vue'
import footer from './components/footer.vue'
import marioAnimation from './components/marioAnimation.vue'

export default {
  components: {
    'app-header': header,
    'app-footer': footer,
    'mario-animation': marioAnimation
  }
}
</script>$

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* width: 900px; */
  height: 768px;
  margin: 0;
  position: relative;
  /* background: #eee; */
}
</style>

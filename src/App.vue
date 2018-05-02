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
html, body, #app {
  height: 100%
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* width: 900px; */
  /* height: 768px; */
  position: relative;
  /* top: 0;
  left: 0;
  bottom: 0;
  right: 0; */
  margin: 0;
  /* background: #eee; */
}
</style>

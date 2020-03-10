<template>
  <div id="app">
    <LeftDiscs/>
    <CenterDisc/>
    <RightDiscs/>
  </div>
</template>

<script>
import LeftDiscs from './components/LeftDiscs.vue'
import CenterDisc from './components/CenterDisc.vue'
import RightDiscs from './components/RightDiscs.vue'

export default {
  name: 'App',
  components: {
    LeftDiscs,
    CenterDisc,
    RightDiscs
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

<template>
  <div id="app">
    <div>
      <Board />
    </div>
    <div class="puzzle-container">
      <LeftDiscs/>
      <CenterDisc/>
      <RightDiscs/>
    </div>
  </div>
</template>

<script>
import LeftDiscs from './components/Board/LeftDiscs.vue'
import CenterDisc from './components/Board/CenterDisc.vue'
import RightDiscs from './components/Board/RightDiscs.vue'

import Board from './components/Numbers/Board.vue';

export default {
  name: 'App',
  components: {
    LeftDiscs,
    CenterDisc,
    RightDiscs,
    Board
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

.puzzle-container {
  position: relative;
  margin-top: 6rem;
}
</style>

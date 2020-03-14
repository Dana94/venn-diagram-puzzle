<template>
  <div id="app">
    <div class="container">
      <div class="numbers-container">
        <Board />
      </div>
      <div class="puzzle-container">
        <LeftDiscs />
        <RightDiscs />
      </div>
    </div>
  </div>
</template>

<script>
import LeftDiscs from './components/Board/LeftDiscs.vue'
import RightDiscs from './components/Board/RightDiscs.vue'

import Board from './components/Numbers/Board.vue';

export default {
  name: 'App',
  components: {
    LeftDiscs,
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
.container {
  display: flex;
  flex-direction: row-reverse;
  width: 80%;
  margin: 0 auto;
}
.puzzle-container {
  /* position: relative;
  width: 80%;
  margin: 6rem auto 0 auto; */

  border: 1px solid black;
  width: 100%;
  height: 30rem;
  display: flex;
  flex-direction: column;
  margin: 0 auto;
  /* order: 2; */
}

.numbers-container {
  width: 100%;
  border: 1px dashed #d0d072;
  /* height: 10rem; */
  /* order: 1; */
}
@media (min-width: 768px) {
  .container {
    display: flex;
    flex-direction: column;
  }
  .puzzle-container {
    /* width: 80%; */
    display: flex;
    flex-direction: row;
    /* order: 2; */
  }

  .numbers-container {
    /* order: 1; */
    height: 10rem;
  }
}
</style>

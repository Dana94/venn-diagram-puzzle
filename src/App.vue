<template>
  <div id="app">
    <div class="container">
      <div class="numbers-container">
        <Board />
      </div>
      <div class="puzzle-container">
        <Discs />
      </div>
    </div>
  </div>
</template>

<script>
import Discs from './components/Board/Discs.vue'
import Board from './components/Numbers/Board.vue';

export default {
  name: 'App',
  components: {
    Discs,
    Board
  }
}
</script>

<style scoped>
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
  height: 90vh;
  border: 1px solid;
}
.puzzle-container {
  position: relative;
  border: 1px dashed green;

  transform-origin: 17rem 14rem;
  transform: rotate(90deg);
}

.numbers-container {
  width: 100%;
  border: 1px dashed #d0d072;
}
@media (min-width: 768px) {
  .container {
    display: flex;
    flex-direction: column;
  }
  .puzzle-container {
    display: flex;
    flex-direction: row;
    justify-content: center;
    transform: rotate(0deg);

  }

  .numbers-container {
    height: 10rem;
  }
}
</style>

<template>
  <div class="right">
    <figure class="figure-1">
      <div class="numbers">
        <div class="number sum10">10</div>
      </div>
    </figure>
    <figure class="figure-2"></figure>
    <figure class="figure-3">
      <div class="numbers">
        <div class="number sum23">23</div>
      </div>
    </figure>
    <figure class="figure-4"></figure>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.number {
  font-size: 25px;
}

.figure-1 .numbers {
  position: relative;
}

.figure-1 .sum10 {
  position: absolute;
  top: 3rem;
  left: 11rem;
}

.figure-3 .sum23 {
  position: absolute;
  bottom: 1rem;
  left: 7rem;
}


figure {
  background-color: transparent;
  height: 15rem;
  width: 15rem;
  border-radius: 50%;
  border: 10px solid black;
}

.figure-1 {
  position: absolute;
  left: 65rem;
  top: 16rem;
}

.figure-2 {
  position: absolute;
  left: 71rem;
  top: 8rem;
}

.figure-3 {
  position: absolute;
  left: 65rem;
  top: 0;
}

.figure-4 {
  position: absolute;
  left: 60rem;
  top: 8rem;
}
</style>

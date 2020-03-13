<template>
  <div class="center">
    <figure class="figure-1">
      <div class="numbers">
        <div class="cap"></div>
        <div class="number sum13">13</div>
      </div>
    </figure>
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
figure {
  background-color: transparent;
  height: 15rem;
  width: 15rem;
  border-radius: 50%;
  border: 10px solid black;
  position: absolute;
  left: 37rem;
  top: 8rem;
}

.number {
  font-size: 25px;
}

.figure-1 .numbers {
  position: relative;
}

.figure-1 .sum13 {
  position: absolute;
  top: 6rem;
  right: 1rem;
}

.cap {
  border-radius: 50%;
  width: 4rem;
  height: 4rem;
  background-color: grey;
  position: absolute;
  left: 5.5rem;
  top: 5rem;
}
</style>

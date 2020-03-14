<template>
  <div class="left">
    <!-- <figure class="figure-1">
      <div class="numbers">
        <div class="cap"></div>
        <div class="number sum10">10</div>
        <div class="number sum05">5</div>
      </div>
    </figure>
    <figure class="figure-2">
      <div class="cap"></div>
    </figure>
    <figure class="figure-3">
      <div class="numbers">
        <div class="cap"></div>
        <div class="number sum07">7</div>
      </div>
    </figure>
    <figure class="figure-4">
      <div class="cap"></div>
    </figure> -->
  </div>
</template>

<script>
export default {
  name: "",
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
  top: 1rem;
  left: 7rem;
}

.figure-1 .sum05 {
  position: absolute;
  top: 3rem;
  left: 3rem;
}

.figure-3 .sum07 {
  position: absolute;
  bottom: 3rem;
  left: 3rem;
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
  left: 20rem;
  top: 16rem;
}

.figure-2 {
  position: absolute;
  left: 28rem;
  top: 16rem;
}

.figure-3 {
  position: absolute;
  /* left: 15rem;
  top: 0; */
  left: 25%;
}

.figure-4 {
  position: absolute;
  left: 10.5rem;
  top: 16rem;
}

.left {
  border: 1px solid #27ef27;

    height: 100%;
}
@media (min-width: 768px) {
  .left {
    width: 50%;
  }
}
.figure-1 .cap {
  border-radius: 50%;
  width: 4rem;
  height: 4rem;
  background-color: grey;
  position: absolute;
  left: 5rem;
  top: 8.5rem;
}

.figure-2 .cap {
  border-radius: 50%;
  width: 4rem;
  height: 4rem;
  background-color: grey;
  position: absolute;
  left: 8rem;
  top: 5.5rem;
}

.figure-3 .cap {
  border-radius: 50%;
  width: 4rem;
  height: 4rem;
  background-color: grey;
  position: absolute;
  left: 5.5rem;
  top: 2.5rem;
}

.figure-4 .cap {
  border-radius: 50%;
  width: 4rem;
  height: 4rem;
  background-color: grey;
  position: absolute;
  left: 2rem;
  top: 5.5rem;
}
</style>

<template>
  <div class="right">
    <!-- <figure class="figure-1">
      <div class="numbers">
        <div class="cap"></div>
        <div class="number sum10">10</div>
      </div>
    </figure>
    <figure class="figure-2">
      <div class="cap"></div>
    </figure> -->
    <figure class="figure-3">
      <div class="numbers">
        <div class="cap"></div>
        <div class="number sum23">23</div>
      </div>
    </figure>
    <figure class="figure-4">
      <div class="cap"></div>
    </figure>
    <figure class="figure-5">
      <div class="numbers">
        <div class="cap"></div>
        <div class="number sum13">13</div>
      </div>
    </figure>
  </div>
</template>

<script>
export default {
  name: "RightDiscs",
  props: {
    msg: String
  }
};
</script>

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

.figure-5 .sum13 {
  position: absolute;
  top: 6rem;
  right: 1rem;
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
  left: 61rem;
  top: 16rem;
}

.figure-2 {
  position: absolute;
  left: 66rem;
  top: 8rem;
}

.figure-3 {
  position: absolute;
  left: 5rem;
  top: -5rem;
}

.figure-4 {
  position: absolute;
  left: 1.5rem;
  top: 6rem;
}
.figure-5 {
  position: absolute;
  left: -10.5rem;
  top: 6rem;
}

.right {
  /* position: absolute;
  top: 0;
  left: -10rem; */
  position: relative;
  border: 1px dashed pink;

    height: 100%;
}

@media (min-width: 768px) {
  .right {
    width: 50%;
  }
}

.cap {
  border-radius: 50%;
  width: 4rem;
  height: 4rem;
  background-color: grey;
  position: absolute;
}

.figure-1 .cap {
  left: 5rem;
  top: 8.5rem;
}

.figure-2 .cap {
  left: 9rem;
  top: 5.5rem;
}

.figure-3 .cap {
  left: 5.5rem;
  top: 2.5rem;
}

.figure-4 .cap {
  left: 4rem;
  top: 5.5rem;
}

.figure-5 .cap {
  left: 5.5rem;
  top: 5rem;
}
</style>

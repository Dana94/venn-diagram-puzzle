<template>
  <div class="sub-container">
    <figure class="figure-1">
      <div class="items">
        <img src="../../assets/slot.svg" id="capA" class="cap" />
        <div class="number sum10">10</div>
        <div class="number sum05">5</div>
      </div>
    </figure>
    <figure class="figure-2">
      <div class="items">
        <img src="../../assets/slot.svg" id="capB" class="cap" />
      </div>
    </figure>
    <figure class="figure-3">
      <div class="items">
        <img src="../../assets/slot.svg" id="capC" class="cap" />
        <div class="number sum07">7</div>
      </div>
    </figure>
    <figure class="figure-4">
      <div class="items">
        <img src="../../assets/slot.svg" id="capD" class="cap" />
      </div>
    </figure>
    <figure class="figure-5">
      <div class="items">
        <img src="../../assets/slot.svg" id="capE" class="cap" />
        <div class="number sum13">13</div>
      </div>
    </figure>
    <figure class="figure-6">
      <div class="items">
        <img src="../../assets/slot.svg" id="capF" class="cap" />
        <div class="number sum10">10</div>
      </div>
    </figure>
    <figure class="figure-7">
      <div class="items">
        <img src="../../assets/slot.svg" id="capG" class="cap" />
      </div>
    </figure>
    <figure class="figure-8">
      <div class="items">
        <img src="../../assets/slot.svg" id="capH" class="cap" />
        <div class="number sum23">23</div>
      </div>
    </figure>
    <figure class="figure-9">
      <div class="items">
        <img src="../../assets/slot.svg" id="capI" class="cap" />
      </div>
    </figure>
  </div>
</template>

<script>
export default {
  name: "",
  mounted() {
    // console.log(document.getElementsByClassName('cap')[0].getBoundingClientRect())
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.sub-container {
  width: 85%;
  position: relative;
}
/* items */

.number {
  font-size: 25px;
}

.figure-1 .items,
.figure-6 .items {
  position: relative;
}

.figure-1 .sum10 {
  position: absolute;
  top: 0rem;
  left: 6rem;
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

.figure-5 .sum13 {
  position: absolute;
  top: 6rem;
  right: 1rem;
}
.figure-6 .sum10 {
  position: absolute;
  top: 3rem;
  left: 9rem;
}

.figure-8 .sum23 {
  position: absolute;
  bottom: 1rem;
  left: 6rem;
}
/* figure */

figure {
  background-color: transparent;
  height: 13rem;
  width: 13rem;
  border-radius: 50%;
  border: 10px solid black;
}

.figure-1 {
  position: absolute;
  left: 5rem;
  top: 14rem;
}

.figure-2 {
  position: absolute;
  left: 10rem;
  top: 7rem;
}

.figure-3 {
  position: absolute;
  left: 5rem;
  top: 0rem;
}

.figure-4 {
  position: absolute;
  left: 0rem;
  top: 7rem;
}

.figure-5 {
  position: absolute;
  left: 20.5rem;
  top: 7rem;
}

.figure-6 {
  position: absolute;
  left: 34.5rem;
  top: 14rem;
}

.figure-7 {
  position: absolute;
  left: 39rem;
  top: 7rem;
}

.figure-8 {
  position: absolute;
  left: 34.5rem;
  top: 0rem;
}

.figure-9 {
  position: absolute;
  left: 30.5rem;
  top: 7rem;
}

.left {
  border: 1px solid #27ef27;
  position: relative;
  height: 100%;
}
@media (min-width: 768px) {
  .left {
    width: 50%;
  }
}

/* caps */
.cap {
  border-radius: 50%;
  width: 4rem;
  height: 4rem;
  background-color: grey;
  position: absolute;
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
  left: 7rem;
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

.figure-5 .cap {
  left: 5.5rem;
  top: 5rem;
}

.figure-6 .cap {
  left: 5rem;
  top: 8.5rem;
}

.figure-7 .cap {
  left: 9rem;
  top: 5.5rem;
}

.figure-8 .cap {
  left: 5.5rem;
  top: 2.5rem;
}

.figure-9 .cap {
  left: 4rem;
  top: 5.5rem;
}

.cap {
  width: 4rem;
  height: 4rem;
}
</style>

<template>
  <!-- <div class="number-token" :value="value">{{value}}</div> -->
  <img src="../../assets/token-1.svg" class="number-token" value="value"/>
</template>

<script>
import {gsap} from 'gsap';
import { Draggable } from "gsap/Draggable";

gsap.registerPlugin(Draggable);

export default {
  props: ['value'],
  data () {
    return {

    }
  },
  mounted() {
    // console.log(document.getElementsByClassName('number-token'))
      Draggable.create(document.getElementsByClassName('number-token'), {
        bounds: document.getElementById('container'),
        type: "x,y",
        liveSnap: {
            //snaps to the closest point in the array, but only when it's within 15px (new in GSAP 1.20.0 release):
            points: [{x: -253, y: 545}],
            radius: 25
        },
        onDragEnd: function () {
          console.log('done', this)
        }
      });
  }
}
</script>

<style scoped>
.number-token {
  width: 4rem;
  height: 4rem;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 1rem;
}

.number-token:hover,
.number-token:focus {
  cursor: pointer;
}
</style>

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
  name: "",
  props: {
    msg: String
  },
  data () {
    return {
      dragged: '',
    }
  },
  methods: {
    onDragOver(event) {
      event.preventDefault();
    },
    onDragLeave(event) {
      event.target.style.background = '';
    },
    onDragEnter(event) {
      const target = event.target;
      if (target) {
          event.preventDefault();
          // Set the dropEffect to move
          event.dataTransfer.dropEffect = 'move'
          target.style.background = '#1f904e';
      }
    },
    onDrop(event) {
      const target = event.target;
      if ( target) {
        target.style.backgroundColor = '';
        event.preventDefault();
        // Get the id of the target and add the moved element to the target's DOM
        this.dragged.parentNode.removeChild(this.dragged);
        this.dragged.style.opacity = '';
        target.appendChild(this.dragged);
      }
    }
  },
  mounted() {
    const dropZone = document.querySelector('.cap');
    dropZone.addEventListener('drop', this.onDrop);
    dropZone.addEventListener('dragenter', this.onDragEnter);
    dropZone.addEventListener('dragleave', this.onDragLeave);
    dropZone.addEventListener('dragover', this.onDragOver);
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

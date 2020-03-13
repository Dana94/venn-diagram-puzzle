<template>
  <div class="number" draggable="true" :value="value">
    {{value}}
  </div>
</template>

<script>
export default {
  props: ['value']
}
</script>

<style scoped>
.number {
  border: 1px solid black;
  border-radius: 50%;
  width: 4rem;
  height: 4rem;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 1rem;
}

.number:hover,
.numbe:focus {
  cursor: pointer;
}
</style>

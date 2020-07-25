<template>
    <div id="numbers-container">
        <Number v-for="i in 1" :key="i.id" :value="i"/>
    </div>
</template>

<script>
import Number from './Number.vue';
export default {
    data () {
        return {
        }
    },
    components: {
        Number
    }
}
</script>

<style>
#numbers-container {
    display: inline-flex;
    justify-content: center;

    border: 1px dashed black;
    height: 6rem;
}
</style>

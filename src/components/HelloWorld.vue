<template>
  <div class="hello">
    <button @click="counter++">Counter value is {{ counter }}</button>
    <p>Counter value passed through computed is {{ computedCounter }}</p>
  </div>
</template>

<script setup>
import { ref } from "vue";

const counter = ref(0);
</script>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  computed: {
    computedCounter() {
      return this.counter;
    },
  },
};
</script>

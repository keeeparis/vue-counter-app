<script lang="ts">
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "Vue Counter App",
    data() {
      return {
        count: 0,
        increase: "Increase Count",
        decrease: "Decrease Count",
      }
    },
    methods: {
      increment() {
        this.count++;
      },
      decrement() {
        this.count--;
      },

    },
  });
</script>
<template>
  <div>
    <h1>Counter</h1>
    <p id="counter">{{ count }}</p>
    <button 
      id="decrease"
      aria-label="decrease button"
      @click="decrement"
    >
      {{ decrease }}
    </button>
    <button 
      id="increase"
      aria-label="increase button"
      @click="increment"
    >
      {{ increase }}
    </button>
  </div>
</template>
<style></style>

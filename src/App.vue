<template>
  <h1>Nuestro primer componente</h1>
  <CarComposition/>
  <CarOptions/>
</template>

<script>
import CarComposition from "./components/CarComposition.vue";
import CarOptions from "./components/CarOptions.vue";

export default {
  components: {
    CarComposition,
    CarOptions,
  },
};
</script>

<style>

</style>

<template>
  <h1>Nuestro primer componente</h1>
  <Car :power="power"/>
</template>

<script>
/* import CarComposition from "./components/CarComposition.vue";
import CarOptions from "./components/CarOptions.vue"; */
import Car from "./components/Car.vue";

export default {
  components: {
    Car,
  },
  setup (){
    let power = 30;

    return {
      power,
    };

  },
};
</script>

<style>

</style>

<template>
  <div class="content">
    <h2 class="title">Coche Compositions Api</h2>
    <p>Marca: {{ brand }}</p>
    <p>Modelo: {{ model }}</p>
    <p>Potencia:</p>
  </div>
</template>

<script>
export default {
  props: {
    power: {
      type: Number,
      default: 60,
    },
  },
  setup(props) {
    const brand = "Audi";
    const model = "A4";
    /*  const power = "40";
    
    const upPower = () => {
      console.log("Aumentar potencia...");
    };

    const downPower = (newPower) => {
      console.log("Disminuir potencia..." + newPower);
    } */

    return {
      brand,
      model,
      /*  power,
      upPower,
      downPower, */
    };
  },
};

/*Asi declaramos una varibale de opciones*/
</script>

<style lang="sass">
.content {
  background: green;

  .title {
    color: red;
  }
}
</style>

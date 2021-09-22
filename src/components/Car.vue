<template>
  <h2>Coche Compositions Api</h2>
  <p>Marca: {{ brand }}</p>
  <p>Modelo: {{ model }}</p>
  <p>Potencia: {{ power }}</p>
  
  
</template>

<script>
export default {
  setup() {
    const brand = "Audi";
    const model = "A4";
    const power = "40";
    
    const upPower = () => {
      console.log("Aumentar potencia...");
    };

    const downPower = (newPower) => {
      console.log("Disminuir potencia..." + newPower);
    }

    return {
      brand,
      model,
      power,
      upPower,
      downPower,
    };
  },
};

/*Asi declaramos una varibale de opciones*/
</script>

<style></style>

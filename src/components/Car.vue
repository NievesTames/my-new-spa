<template>
  <h2>Coche</h2>
  <p>Marca: {{ brand }}</p>
  <p>Modelo: {{ model }}</p>
  <!-- <p>Color: {{ color[1] }}</p> -->
  <p>
      Color: 
      <!-- <span v-for="(color, index) in colors" :Key="index">
          {{ index }} : {{ color }} -
      </span> -->
  </p>
  <ul>
      <li v-for="(color, index) in colors" :Key="index">
          {{ index }} : {{ color }}
      </li>
  </ul>
  <p>Precio: {{ price }}</p>
  <p>Potencia: {{ power}}CV</p>
  {{ mensaje.title }} - {{ mensaje.text }}
</template>

<script>
export default {
    /* data(){
        return {
            brand: "Audi",
            model: "A4",
            color: ["Negro", "Verde", "Azul"],
            price: 35000, 
            power:180,
            mensaje: {
                title: "Hola mundo",
                text: "Adios",
            }
        };
    }, */
    setup (){
        const brand = "Audi";
        const model = "A4";
        const colors = ["Azul", "Morado", "Marrón", "Amarillo"];
        const price = 450000;
        const power = 240;
        const mensaje = {
            title: "Estoy bien",
            text: "Por fin con Vue",
        };

    return {
        brand,
        model,
        colors,
        price,
        power, 
        mensaje,
    };
 },
};

/*Asi declaramos una varibale de opciones*/

</script>

<style>

</style>


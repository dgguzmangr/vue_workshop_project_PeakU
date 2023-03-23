<template>
  <div class="hello">
    <h1>{{ msg }} {{ numero }}</h1>
    {{ mivariable }}
    <br>
    <br>

    <h2>Directiva v-for</h2>

    <ul>
      <li v-for="(fruta, index) in frutas" :key="index">
        {{ index }} - {{ fruta.nombre }} - {{ fruta.cantidad }}
          <p v-show="fruta.cantidad >= 5">
            Hay 5 o más
          </p>

          <p v-show="fruta.cantidad <= 5">
            Hay 5 o menos
          </p>
      </li>
    </ul>
    <p>
      For a guide and recipes on how to configure / customize this project,<br>
      check out the
    </p>
      
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    numero: Number
  },
  data() {
    return {
      mivariable: "fgfdsghfhgfhgfhj",
      frutas: [
        {
          nombre: "Manzana",
          cantidad: 5
        },
        {
          nombre: "Peras",
          cantidad: 2
        },
        {
          nombre: "Duraznos",
          cantidad: 6
        },
        {
          nombre: "Banano",
          cantidad: 5
        }
    ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

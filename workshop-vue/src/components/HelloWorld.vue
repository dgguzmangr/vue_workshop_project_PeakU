<template>
  <div class="hello">
    <h1>{{ msg }} {{ numero }}</h1>
    {{ mivariable }}
    <br>
    <br>

    <h2>Directiva v-for</h2>

    <ul>
      <li v-for="(job, index) in JobListing" :key="index">
        {{ job.jobTitle }} - {{ job.company }} {{ job.salary }}
      </li>
    </ul>
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
      ],

      JobListing: [
        {
          jobTitle: "Ingeniero de datos",
          company: "Fourier Analytics",
          salary: "$ 1.4M COP"
        },
        {
          jobTitle: "Devops",
          company: "Aventior Inc",
          salary: "$ 1.2M COP"
        },
        {
          jobTitle: "Analista QA",
          company: "Be Bolder",
          salary: "$ 6.1M COP"
        },
        {
          jobTitle: "Auxiliar de odontología",
          company: "WOWaligners SAS",
          salary: "$ 1.2M COP"
        },
        {
          jobTitle: "Desarrollador",
          company: "Zona Virtual",
          salary: "$ 3.8M COP"
        },
        {
          jobTitle: "Auxiliar administrativa y de logística",
          company: "Magno Chocolates",
          salary: "$ 1.2M COP"
        },
        {
          jobTitle: "Ingeniero Devops bilingue",
          company: "PeakU",
          salary: "$ 6K USD"
        },
        {
          jobTitle: "Gerente comercial de licitaciones con el estado",
          company: "Confidencial",
          salary: "$ 7M COP"
        },
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

<template>
  <div class="mx-auto container-fluid bg-light">
    <div  v-for="(job, index) in JobListing" :key="index" class="jobpost card-body row d-flex justify_content-center align-items-center text-center p-3  m-3 border border-muted rounded">
      <div class="justify-content-center align-items-center col-md-1 col-3">
        <div style="width: 70px; height: 70px" class="rounded img-fluid">
          <img :src="job.img" alt="company logo" width="70" height="70" class="rounded">
        </div>
      </div>
      <div class="col-md-11 col-9 row align-items-start">
        <div class="row align-items-center ">
          <a href="" class="text-dark d-inline d-md-inline-flex fw-bold text-decoration-none">{{ job.jobTitle }}</a>
        </div>
        <div class="jobitems row pl-md-2 mt-1 flex column flex-md-row">
          <div class="text-truncate text-capitalize col ">
            <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="building" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-building b-icon bi"><g data-v-03976c49=""><path fill-rule="evenodd" d="M14.763.075A.5.5 0 0 1 15 .5v15a.5.5 0 0 1-.5.5h-3a.5.5 0 0 1-.5-.5V14h-1v1.5a.5.5 0 0 1-.5.5h-9a.5.5 0 0 1-.5-.5V10a.5.5 0 0 1 .342-.474L6 7.64V4.5a.5.5 0 0 1 .276-.447l8-4a.5.5 0 0 1 .487.022zM6 8.694 1 10.36V15h5V8.694zM7 15h2v-1.5a.5.5 0 0 1 .5-.5h2a.5.5 0 0 1 .5.5V15h2V1.309l-7 3.5V15z"></path><path d="M2 11h1v1H2v-1zm2 0h1v1H4v-1zm-2 2h1v1H2v-1zm2 0h1v1H4v-1zm4-4h1v1H8V9zm2 0h1v1h-1V9zm-2 2h1v1H8v-1zm2 0h1v1h-1v-1zm2-2h1v1h-1V9zm0 2h1v1h-1v-1zM8 7h1v1H8V7zm2 0h1v1h-1V7zm2 0h1v1h-1V7zM8 5h1v1H8V5zm2 0h1v1h-1V5zm2 0h1v1h-1V5zm0-2h1v1h-1V3z"></path></g></svg>
            <span>{{ job.company }}</span>
          </div>
          <div class="text-truncate col">
            <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="geo alt" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-geo-alt b-icon bi"><g data-v-03976c49=""><path d="M12.166 8.94c-.524 1.062-1.234 2.12-1.96 3.07A31.493 31.493 0 0 1 8 14.58a31.481 31.481 0 0 1-2.206-2.57c-.726-.95-1.436-2.008-1.96-3.07C3.304 7.867 3 6.862 3 6a5 5 0 0 1 10 0c0 .862-.305 1.867-.834 2.94zM8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10z"></path><path d="M8 8a2 2 0 1 1 0-4 2 2 0 0 1 0 4zm0 1a3 3 0 1 0 0-6 3 3 0 0 0 0 6z"></path></g></svg>
            <span>{{ job.city }}</span>
          </div>
          <div class="text-truncate col">
            <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="cash" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-cash b-icon bi"><g data-v-03976c49=""><path d="M8 10a2 2 0 1 0 0-4 2 2 0 0 0 0 4z"></path><path d="M0 4a1 1 0 0 1 1-1h14a1 1 0 0 1 1 1v8a1 1 0 0 1-1 1H1a1 1 0 0 1-1-1V4zm3 0a2 2 0 0 1-2 2v4a2 2 0 0 1 2 2h10a2 2 0 0 1 2-2V6a2 2 0 0 1-2-2H3z"></path></g></svg>
            <span>{{ job.salary }}</span>
          </div>
          <div class="d-inline-flex text-truncate col">
            <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="people" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-people b-icon bi"><g data-v-03976c49=""><path d="M15 14s1 0 1-1-1-4-5-4-5 3-5 4 1 1 1 1h8zm-7.978-1A.261.261 0 0 1 7 12.996c.001-.264.167-1.03.76-1.72C8.312 10.629 9.282 10 11 10c1.717 0 2.687.63 3.24 1.276.593.69.758 1.457.76 1.72l-.008.002a.274.274 0 0 1-.014.002H7.022zM11 7a2 2 0 1 0 0-4 2 2 0 0 0 0 4zm3-2a3 3 0 1 1-6 0 3 3 0 0 1 6 0zM6.936 9.28a5.88 5.88 0 0 0-1.23-.247A7.35 7.35 0 0 0 5 9c-4 0-5 3-5 4 0 .667.333 1 1 1h4.216A2.238 2.238 0 0 1 5 13c0-1.01.377-2.042 1.09-2.904.243-.294.526-.569.846-.816zM4.92 10A5.493 5.493 0 0 0 4 13H1c0-.26.164-1.03.76-1.724.545-.636 1.492-1.256 3.16-1.275zM1.5 5.5a3 3 0 1 1 6 0 3 3 0 0 1-6 0zm3-2a2 2 0 1 0 0 4 2 2 0 0 0 0-4z"></path></g></svg>
            <span class="d-inline">
              {{ job.vacant }}
              <span v-if="job.vacant === 1" class="ml-1">vacante</span>
              <span v-else class="ml-1">vacantes</span>
            </span>
          </div>
          <div class="text-truncate col">
            <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="calendar3" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-calendar3 b-icon bi"><g data-v-03976c49=""><path d="M14 0H2a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2zM1 3.857C1 3.384 1.448 3 2 3h12c.552 0 1 .384 1 .857v10.286c0 .473-.448.857-1 .857H2c-.552 0-1-.384-1-.857V3.857z"></path><path d="M6.5 7a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm-9 3a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm-9 3a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2z"></path></g></svg>
            <span class="job-date">{{ job.date }}</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
  
<script>
export default {
  name: 'JobOffer',
  data() {
    return {
      JobListing: [
        {
          img: "https://peaku.co/img/company.svg",
          jobTitle: "Regente de farmacia",
          company: "OFFIMÉDICAS S.A",
          city: "Santiago de Cali",
          salary: "$ 1.9M COP",
          vacant: 10,
          date: "2023-02-25",
        },
        {
          img:"https://s3-us-west-2.amazonaws.com/peaku-public/business/Company/logo_url/40668/descarga.png",
          jobTitle: "Ingeniero de datos",
          company: "Fourier Analytics",
          city: "Remoto en Colombia",
          salary: "$ 6.5M - 8M COP",
          vacant: 5,
          date: "2023-03-25",
        },
        {
          img:"https://s3-us-west-2.amazonaws.com/peaku-public/business/Company/logo_url/70785/Aventior_Inc.jpg",
          jobTitle: "Devops",
          company: "Aventior Inc",
          city: "Remoto",
          salary: "$ 4M - 6.1M COP",
          vacant: 1,
          date: "2023-01-05",
        },
      ],
      show: 1
    }
  },
  methods: {
    toggleShow() {
      this.show = !this.show;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
:root {
  --borderColor: #212529;
}


h4 {
  font-weight: bold;
  color: #343a40;
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
span {
  font-size: 0.75rem;
  padding-left: 0.5em;
  display: inline-block;
}
p {
  margin-bottom: 0;
}
.jobitems {
  text-align: left;
}

.jobitems {
  text-align: left;
  display: flex; /* Utiliza flexbox */
  align-items: center; /* Centra verticalmente el contenido */
}

.jobpost:hover {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2); /* Agregar una sombra cuando se pasa el ratón */
}
</style>
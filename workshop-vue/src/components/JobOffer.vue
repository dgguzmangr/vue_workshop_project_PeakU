<template>
  <ul>

    
    <li v-for="(job, index) in JobListing" :key="index" class="border rounded shadow">

      <a href="">
        <div class="row d-flex justify_content-center align-items-center text-center">

          <div class="col">
            <img :src="job.img" alt="company logo">
          </div>

          <div class="col">

            <div class="row d-flex justify_content-center align-items-center text-center">
              <h4>{{ job.jobTitle }}</h4>
            </div>

            <div class="row d-flex justify_content-center align-items-center text-center">
              <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="building" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-building b-icon bi"><g data-v-03976c49=""><path fill-rule="evenodd" d="M14.763.075A.5.5 0 0 1 15 .5v15a.5.5 0 0 1-.5.5h-3a.5.5 0 0 1-.5-.5V14h-1v1.5a.5.5 0 0 1-.5.5h-9a.5.5 0 0 1-.5-.5V10a.5.5 0 0 1 .342-.474L6 7.64V4.5a.5.5 0 0 1 .276-.447l8-4a.5.5 0 0 1 .487.022zM6 8.694 1 10.36V15h5V8.694zM7 15h2v-1.5a.5.5 0 0 1 .5-.5h2a.5.5 0 0 1 .5.5V15h2V1.309l-7 3.5V15z"></path><path d="M2 11h1v1H2v-1zm2 0h1v1H4v-1zm-2 2h1v1H2v-1zm2 0h1v1H4v-1zm4-4h1v1H8V9zm2 0h1v1h-1V9zm-2 2h1v1H8v-1zm2 0h1v1h-1v-1zm2-2h1v1h-1V9zm0 2h1v1h-1v-1zM8 7h1v1H8V7zm2 0h1v1h-1V7zm2 0h1v1h-1V7zM8 5h1v1H8V5zm2 0h1v1h-1V5zm2 0h1v1h-1V5zm0-2h1v1h-1V3z"></path></g></svg>
              {{ job.company }}
              <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="cash" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-cash b-icon bi"><g data-v-03976c49=""><path d="M8 10a2 2 0 1 0 0-4 2 2 0 0 0 0 4z"></path><path d="M0 4a1 1 0 0 1 1-1h14a1 1 0 0 1 1 1v8a1 1 0 0 1-1 1H1a1 1 0 0 1-1-1V4zm3 0a2 2 0 0 1-2 2v4a2 2 0 0 1 2 2h10a2 2 0 0 1 2-2V6a2 2 0 0 1-2-2H3z"></path></g></svg>
              {{ job.salary }}
            </div>

          </div>
          <div class="col">

          </div>
        </div>
      </a>
      
    </li>
  </ul>
</template>
  
  <script>
  export default {
    name: 'JobOffer',
    data() {
      return {
        JobListing: [
          {
            img: "./assets/ss.png",
            jobTitle: "Regente de farmacia",
            company: "OFFIMÉDICAS S.A",
            salary: "$ 1.9M COP"
          },
        ]
      }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
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
  </style>
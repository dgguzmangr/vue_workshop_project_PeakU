<template>
  <div id="app">
    <nav class="container">
                <!--section typeA (four columns, each colum img[align items center] + <p> under the img[align items left] )-->
                <section class="row d-flex justify-content-center align-items-center text-center py-3" style="background-color: var(--white);">
                    <div class="col text-left">
                        <a href="index.html"><img loading="lazy" src="./assets/logo-blue.png" alt="PeakU"></a>
                    </div>
                    <div class="col text-center">
                        <div class="d-flex justify-content-between row list-unstyled font-weight-bold"
                            style="font-family: var(--primaryFont); color: var(--colorB-1);">
                            <li><a href="#" class="text-decoration-none text-reset">Empleos</a></li> <!--vínculo-->
                            <li><a href="#" class="text-decoration-none text-reset">Bootcamp</a></li> <!--vínculo-->
                            <li><a href="#" class="text-decoration-none text-reset">Acerca de nosotros</a></li> <!--vínculo-->
                            <li><a href="#" class="text-decoration-none text-reset">Para profesionales</a></li> <!--vínculo-->
                            <li><a href="#" class="text-decoration-none text-reset">Para empresas</a></li> <!--vínculo-->
                        </div>
                    </div>
                    <div class="col text-right">
                        <button class="btn1 float-right">Español</button>
                        <button class="btn1 float-right">Notificaciones</button>
                        <button class="btn2 float-right">Login</button>
                    </div>
                </section>
            </nav>
    <JobOffer/>
  </div>
</template>

<script>
import JobOffer from './components/JobOffer.vue';

export default {
  name: 'App',
  components: {
    JobOffer
  }
}
</script>

<style>
#app {
  font-family: sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #212529;
  margin-top: 60px;
}
</style>

<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero illo harum, architecto porro, voluptas a vel commodi quibusdam veniam in optio voluptatem totam. Sequi maxime veniam veritatis soluta eveniet in?</p>

    <HelloWorld msg="Hola" :numero="5"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

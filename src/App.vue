<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <BotaoPrincipal :texto="'Botao 1'" />
    <BotaoPrincipal :texto="'Não clique aqui'" />
    <BotaoPrincipal corDoBotao="blue" corDoTexto="white"/>
    <BotaoPrincipal corDoBotao="red" />
    <BotaoPrincipal corDoBotao="#a8a632" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import BotaoPrincipal from "./components/BotaoPrincipal.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    BotaoPrincipal
  }
};
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

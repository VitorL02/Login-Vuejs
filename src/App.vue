
<template>
  <div id="app">
    <LoginMensage></LoginMensage>
    <LoginInputs></LoginInputs>
  </div>
</template>



<script >
import LoginMensage from './components/LoginMensage.vue'
import CardLogin from './components/CardLogin.vue'
import LoginInputs from './components/LoginInputs.vue';
export default {

  name: 'App',
  components: {
    LoginMensage,
    CardLogin,
    LoginInputs
  }

}


</script>

<style>
#app {
  width: 100vw;
  height: 100vh;
  background: #201b2c;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>

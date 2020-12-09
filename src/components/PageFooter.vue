<template>
  <footer class="footer col-md-12 mt-4 text-center">
    <div id="PageFooter"></div>
    <div class="row text-light">
      <div class="col-md-6">
        <p text-align: center>
          Presentación trabajo semana 2 - Ciclo 3 Desarrollo de Software.
        </p>
        <p>
          Motivación: Entender y aprender a utilizar herramientas de desarrollo
          WEB.
        </p>
        <p>https://github.com/MinTicGrupo149/semana-1-149</p>
      </div>
      <div class="col-md-6">
        <p>
          Jesús Rivas (Desarrollador Front-END - Tester):
          rivas.jesus93@gmail.com
        </p>
        <p>Juan Pabón (Desarrollador Backend - Tester): juanfpc@hotmail.com</p>
        <p>
          Santiago Monsalve (Arquitecto de Software - Tester):
          samonsalvebo@gmail.com
        </p>
        <p>
          Esteban Madrid (Analista de Software - Tester): samonsalvebo@gmail.com
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "PageFooter",
  props: ["member"],
  data() {
    return {
      title: "Footer",
    };
  },
};
</script>

<style scoped>
</style>
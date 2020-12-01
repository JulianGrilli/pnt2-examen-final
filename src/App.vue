<template>
  <div id="app">
    <EjercicioFinal />
    <table class="table">
  <thead>
    <tr>
      <th scope="col">Numero de pregunta</th>
      <th scope="col">Respuesta</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>B</td>
    </tr>
    <tr>
      <td>2</td>
      <td>C</td>
    </tr>
    <tr>
      <td>3</td>
      <td>B</td>
    </tr>
    <tr>
      <td>4</td>
      <td>D</td>
    </tr>
    <tr>
      <td>5</td>
      <td>D</td>
    </tr>
  </tbody>
</table>
  </div> 
</template>

<script>
import EjercicioFinal from '../src/components/EjercicioFinal.vue'
export default {
  name: 'App',
  components: {
    EjercicioFinal
  }
}
</script>

<style>
  #app {
  }

  table{
    margin-top: 50px;
  }
</style>

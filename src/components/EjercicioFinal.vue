<template>

  <section class="src-components-ejercicio-final">
    Color: <input type="text" v-model="colorTexto" style="margin:10px;" >
    Fondo: <input type="text" v-model="fondoTexto" style="margin:10px;" >
    Size: <input type="text" v-model="sizeTexto" style="margin:10px;" >
    <br>
    <hr>
    Texto: <input type="text" 
    :style="{ color: colorTexto, backgroundColor: fondoTexto, fontSize: sizeTexto }"
    v-model="mensaje" style="margin:10px;" >
    <br>
    <br>
    <span v-if="contarPalabras > 0"><strong>Cantidad de palabras:</strong> {{contarPalabras}}</span>
  </section>

</template>

<script>
  export default  {
    name: 'src-components-ejercicio-final',
    props: [],
    mounted () {
      
    },
    data () {
      return {
        colorTexto : '',
        fondoTexto : '',
        sizeTexto : '',
        mensaje: ''
      }
    },
    methods: {
      
    },
    computed: {
      contarPalabras(){
        const arrayMessage = this.mensaje.split(' ');
        let arrayFinal = []
        arrayMessage.forEach(palabra => {
          if(palabra != ""){
            arrayFinal.push(palabra)
          }
        })
        return arrayFinal.length;
      },
    }
}


</script>

<style scoped lang="css">
  .src-components-ejercicio-final {
    margin-left: 20px;
  }
  .mensajeSpan{
    margin-left: 10px;
  }
</style>

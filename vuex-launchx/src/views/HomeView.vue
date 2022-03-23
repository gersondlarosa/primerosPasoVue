<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">

    <Contador/>
    <Cuadrado/>
    <Botones/>



  </div>
</template>

<script>
import Contador from "../components/contador.vue"
import Cuadrado from "../components/cuadrado.vue"
import Botones from "../components/botones.vue"
export default {

  name: 'HomeView',
  components:{
    Contador,
    Cuadrado,
    Botones
  }
  //se quita data ya que se obtendra del estado en store el contador
/*  data(){
    return {
      /*Para regresar se nesesita un objeto { contador:0}
      contador: 0
    }

  methods: {
    bajarContador(){
      this.contador--;
    },
    subirContador(){
      this.contador++;
    }
  }*/
}
</script>

<style>

div{
  margin-bottom: 10px;
}
  .contador{
    font-size: 80px;
  }
  .botones button{
    font-size: 40px;
    width: 100px;
    margin: 0 10px;
  }
  .cuadrado{
    font-size: 25px;
  }
</style>

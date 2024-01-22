<script>
  export default{
    data: () => ({
      contador: 10
    }),
    methods: {
      aumentar(){
        this.contador++;
      },
      disminuir(){
        this.contador--;
      },
      reset(){
        this.contador=10;
      }
    }
  }
</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="logo vue" width="125" height="125">
    <br>
    <h1>Hola mundo</h1>
    <hr/>
    <h2>Contador: {{ contador }}</h2>
    <button @click="aumentar()">+</button>
    <button @click="disminuir()">-</button>
    <button @click="reset()">Reset</button>
  </div>
</template>

<style scoped>
  .container{
    text-align: center;
  }
  h1{
    font-weight: bolder;
  }
  button{
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 6px;
    width: 150px;
  }
</style>
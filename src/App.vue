<script>
export default {
  data(){
    return{
      contador:0,
    }
  },
  methods:{
    incrementar(){
      this.contador++;
    },
    decrementar(){
      this.contador--;
    },
    reset(){
      this.contador = 0;
    }

  },
}
</script>

<template>
  <div class="container">
    <img src=".\assets\logo.svg" alt="Logo VUE" width="100" height="100" />
  <small>
    <h1>Hola desde Vue JS</h1>
  </small>
  
  <hr />

  <h2>Contador: {{contador}}</h2>
  <button @click="incrementar()">+1</button>
  <button @click="decrementar()">-1</button>
  <button @click="reset()">reset</button>
  </div>
  
</template>

<style scoped>

.container{
  text-align: center;
  
}
h1{
  font-weight: bolder;
}
small{
  color: blue;
}

h2{
  font-size: 2.5rem;
}

button{
  cursor: pointer;
  font-size: 2.5rem;
  margin: 0px 6px;
}
</style>

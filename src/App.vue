<template>
  <!-- <HelloWorld/> -->
  <Quiz8/>

  <div class="app">
    <h1>Nama saya {{ name }}</h1>
    <h2>{{ bilangan }}</h2>
    <button v-on:click="tambah">Tambah</button>
    <button v-on:click="kurang">Kurang</button>
    <button v-on:click="kali">Kali</button>
    <button v-on:click="bagi">bagi</button>
</div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Quiz8 from './components/Quiz8.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    Quiz8,
  },

  data(){
    return{
      name : "Kenedi Fagus Pradana",
      bilangan : 1,
    }
  },

  methods: {
    tambah(){
      this.bilangan += 1;
    },
    kurang(){
      this.bilangan -= 1;
    },
    kali(){
      this.bilangan *= 5;
    },
    bagi(){
      this.bilangan /= 5;
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.app{
  text-align: center;
  justify-content: center;
  margin-bottom: 20px;
}

h2{
  color: red;
}

button{
  margin: 5px;
  background-color: #B6E2A1;
  border-radius: 10px;
}
</style>

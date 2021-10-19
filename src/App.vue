<template>
<div>
  {{users}}
  <ul>
    <li :key="meyve" v-for="(meyve,key) in meyveler">{{key+meyve}}</li>
  </ul>
</div>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Mijn eerste Vue.js Project"/>
  <my-button></my-button>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MyButton from './components/MyButton.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    MyButton
  },
  data () {
    return {
      users: 'Mehmet',
      meyveler: ['ali', 'erma', 'xvvcx']
    }
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

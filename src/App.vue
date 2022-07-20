<template>
  <div id="app">
    {{ fname }} {{ name }} {{key}}
    <div v-text="lname"></div>
    <img alt="Vue logo" src="https://vuejs.org/images/logo.png" />
  </div>
  
  <h2 v-if="num===6">Number is 6</h2>
  <h2 v-else="num>0">NUmber is Null<h2>
   <h2 v-else="num<0">The number is Zero</h2>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import Hayat from './components/Hayat.vue';

export default {
  name: 'App',
  data() {
    return {
      fname: 'Hayat',
      name: 'Batman',
      lname: 'King',
      num:3
    };
  },
  components: {
    // HelloWorld
    Hayat,
  },
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
.new{
  color:purple;
}
.sold-out {
  color: red;
}
</style>

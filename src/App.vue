<template>
  <div id="app">

      <h1>Parent</h1>
      <button @click="selected='app-bike'">Bike</button>
      <button @click="selected='app-rikshaw'">Rikshaw</button>
      <button @click="selected='app-car'">Car</button>

      
<br>
      <keep-alive>
      <component style="height: 500px" :is="selected"> </component>
      </keep-alive>
    </div>
</template>

<script>
import Bike from'./components/Bike';
import Car from'./components/Car';
import Rikshaw from'./components/Rikshaw';

export default {
  name: 'app',
  components: {
    'app-bike': Bike,
    'app-car': Car,
    'app-rikshaw': Rikshaw
  
  },

  data(){
    return{
      counter:0,
      selected:'app-rikshaw'
    }
  }

}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: azure; 
  margin-top: 60px;
}
</style>

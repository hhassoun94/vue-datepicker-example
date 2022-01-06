<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <div class="container">
    <div class="row justify-content-center my-4">
      <div class="col-8">
        <h1>vue3-datepicker</h1>
        <Datepicker1 class="w-100" v-model="date"/>
      </div>
    </div>
    <div class="row justify-content-center my-4">
      <div class="col-8">
        <h1>vue3-date-time-picker</h1>
        <Datepicker2 class="w-100" v-model="date"/>
      </div>
    </div>
    <div class="row justify-content-center my-4">
      <div class="col-8">
        <h1>Native HTML datepicker</h1>
        <input class="form-control w-100" type="date" name="" id="" v-model="date">
      </div>
    </div>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Datepicker1 from 'vue3-datepicker'
import Datepicker2 from 'vue3-date-time-picker'
import 'vue3-date-time-picker/dist/main.css'
import 'bootstrap/dist/css/bootstrap.min.css'
import 'bootstrap'

export default {
  name: 'App',
  data(){
    return {
      date: new Date()
    }
  },
  components: {
    Datepicker1,
    Datepicker2
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

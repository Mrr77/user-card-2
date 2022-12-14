<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App" :name="name" :photo="photo" :fio="fio" :adress="adress" :email="email" :phone="phone"/>
</template>

<script>
import { tsImportEqualsDeclaration } from '@babel/types';
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  one(){
    photo: "";
    name: "";
    fio: "";
    adress: "";
    email: "";
    phone: ""

  },
  two(){
    this.axios.get('').
    then((response) => {console.log(response.data), this.name = "ll", this.photo = "ll", this.fio = "ll", this.adress = "ll", this.email = "ll", this.phone = "ll"}
  )}
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

<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <input type="text" v-model="name" >
    <div>{{name}}</div>
    <div style="color:red;" v-show="show"> ẨN HIỆN </div> <br>
    <button @click="show = !show">Ấn</button>
    <div  :class="{class: chon}"> ẨN HIỆN </div> <br>
    <button @click="chon = !chon">Ấn</button>
  </div>
</template>

<script>
export default {

  data(){
    return{
      name: 'Tuấn dz',
      show: true,
      chon: true
    }
  },
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
.class{
  color: red;
}
</style>

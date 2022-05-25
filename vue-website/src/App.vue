<template>
  <div id="app">
    <home />
  </div>
</template>

<script>
import home from './components/home.vue'

export default {
  name: 'App',
  components: {
    home
  },
  created(){
    console.log("b" + "a" + +"a" + "a");
  }
}
</script>

<style>
#app {
  font-family: 'Nunito Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100vw;
  max-width: 100%;
}
button{
  font-family: 'Nunito Sans', sans-serif;
  font-weight: 700;
}
button:hover{
  cursor: pointer;
}
svg{
  height: 30px;
}
svg g path{
  fill: rgb(44, 62, 80);
}
ul{
  padding: 0;
  list-style-type: none;
}
a{
  color: rgb(44, 62, 80);
}
a:hover{
  cursor: pointer;
  color: orange;
}
*:before,
*:after {
  box-sizing: border-box;
}
*:focus {
  outline: none;
}
*{
  padding:0;
  margin:0;
  box-sizing: border-box;
}
</style>

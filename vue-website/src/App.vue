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
}
button{
  font-family: 'Nunito Sans', sans-serif;
  font-weight: 700;
}
button:hover{
  cursor: pointer;
}
svg{
  height: 50px;
}
svg g path{
  fill: rgb(44, 62, 80);
}
*:before,
*:after {
  box-sizing: border-box;
}
*:focus {
  outline: none;
}
</style>

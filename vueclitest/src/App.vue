<template>
  <div id="app">
    <img src="./assets/logo.png">
    <div>
      <router-link to="/" >首页</router-link> |
      <router-link to="/Hi">Hi页面</router-link> |
      <router-link :to="{name:'Hi1',params:{username:'Coldcode',id:'627'}}" >Hi1</router-link> |
      <router-link to="/Hi/Hi2" >Hi2</router-link>
    </div>
    <p>{{ $route.name }}</p>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

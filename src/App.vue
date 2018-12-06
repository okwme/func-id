<template>
  <div id="app">
    <a href="https://clovers.network">
      <img src="https://clovers.network/img/icons/android-chrome-512x512.png">
    </a>
    <h1>Welcome</h1>
    <h2>Convert your function to it's corresponding ethereum function identifier</h2>
    <HelloWorld/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
body, html {
  padding: 0;
  margin:0;
}
* {
  box-sizing: border-box;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  max-width: 380px;
  padding:5px;
  margin: 60px auto 0 auto;
}
img {
  width: 100%;
  max-width: 280px;
}
</style>

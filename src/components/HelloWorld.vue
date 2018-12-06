<template>
  <div class="hello">
    <input placeholder="functionName(parameter)" v-model="functionName"/><br>
    <input placeholder="function identifier" readonly v-model="identifier"/><br>
  </div>
</template>

<script>
import utils from 'web3-utils'
export default {
  name: 'HelloWorld',
  data () {
    return {
      functionName: ''
    }
  },
  computed: {
    identifier () {
      if (!this.functionName) return ''
      return utils.sha3(this.functionName).substr(0, 10)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
input {
font-size: 28px;
line-height: 1.2em;
padding:5px;
margin: 5px auto;
width: 100%;
max-width:380px;
  
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

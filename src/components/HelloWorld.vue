<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>by -env107</h2>
  </div>
</template>

<script>
import {mapState} from "vuex"
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Vue 构建项目' + this.$store.getters.version,
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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

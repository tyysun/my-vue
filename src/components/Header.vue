<template>
  <header>
    <h1>{{title}}</h1>
  </header>
</template>

<script>
export default {
  name: 'app-header',
  data () {
    return {
      title:'这是我的第一个 Vue.js Demo'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header{
  background: rgb(24, 209, 178);
  padding: 10px;
  text-align: center;
}
h1{
  color: #222;
}
</style>

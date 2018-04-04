<template>
  <footer>
    <h1>{{copyright}}</h1>  
  </footer>
</template>

<script>
export default {
  name: 'app-footer',
  data () {
    return {
      copyright: 'Copyright 2017 Vue Demo'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
footer{
  background: rgb(15, 97, 219);
  padding: 10px;
  text-align: center;
}
h1{
  color: #222;
}
</style>

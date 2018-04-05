<template>
  <footer>
    <p>{{copyright}}</p>  
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
  padding: 5px;
  text-align: center;
}

</style>

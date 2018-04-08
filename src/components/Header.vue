<template>
  <header>
    <h1 v-on:click="changeTitle">{{title}}</h1>
  </header>
</template>

<script>
export default {
  name: 'app-header',
  props:{
    title:{type:String,
    require:true

    }},
  data () {
    return {
      // title:'这是我的第一个 Vue.js Demo'
    }
  },
  methods:{
    changeTitle:function(){
      this.$emit('changeTitle1','事件传值')
      // 事件传值注意各参数代表的含义
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

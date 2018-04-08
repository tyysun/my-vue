<template>
  <div id="app">
    
    <ul>
      <li><router-link to='/'>Home</router-link></li>
      <li><router-link to='/helloworld'>helloworld</router-link></li>
    </ul>
   <router-view></router-view>
  </div>
</template>
// 注意属性传值中a与b分别代表什么
<script>


export default {
  name: 'App',
  data(){
    return {}
      
  },
  components: {
    
  },
 
}
</script>

<style>

</style>

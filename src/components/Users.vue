<template>
  <div class="users">
    <ul>
      <!-- <li v-for="user in a" v-on:click = "user.show=!user.show">
          <h2>{{user.name}}</h2>
          <h3 v-show='user.show'>{{user.position}}</h3>
      </li> -->
      <li v-for="user in a">
          <h2>{{user.name}}</h2>
          <h3>{{user.email}}</h3>

      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'users',
  props:{
    a:{type:Array,
    require:true

    }
  },
  data () {
    return {
      
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.users{
  width: 100%;
  max-width: 1200px;
  margin: 40px auto;
  box-sizing: border-box;

}
ul{
  display: flex;
  flex-wrap: wrap;
  list-style: none;
}
li{
  flex-grow: 1;
  flex-basis: 200px;
  text-align: center;
  border: 1px solid #222;
  padding: 30px;
  margin:10px;
}

</style>

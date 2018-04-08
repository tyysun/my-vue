<template>
  <div id="home">
    <app-header v-bind:title="title" v-on:changeTitle1="updataTitle($event)"></app-header>
    <users v-bind:a='b'></users>
    <app-footer></app-footer>  
   
  </div>
</template>
// 注意属性传值中a与b分别代表什么
<script>
import Users from './Users'
import Header from './Header'
import Footer from './Footer'

export default {
  name: 'home',
  data(){
    return {
       b: [
      //{name:"Tim",position:'前端工程师',show:false},
      //         {name:"Tim",position:'前端工程师',show:false},
      //         {name:"Tim",position:'前端工程师',show:false},
      //         {name:"Tim",position:'前端工程师',show:false},
      //         {name:"Tim",position:'前端工程师',show:false},
      //         {name:"Tim",position:'前端工程师',show:false},
      //         {name:"Tim",position:'前端工程师',show:false},
      //         {name:"Tim",position:'前端工程师',show:false}
      ],
      title:'我是小标题'
    }
  },
  components: {
    'users':Users,
    'app-header':Header,
    'app-footer':Footer
  },
  methods:{
    updataTitle:function(a){
        this.title=a;
    }
  },
  created(){
    this.$http.get("http://jsonplaceholder.typicode.com/users")
        .then((data) => {
          console.log(data);
          this.b = data.body;
        })
  }
}
</script>

<style>

</style>

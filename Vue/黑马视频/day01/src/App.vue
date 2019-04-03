<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>{{ msg }}</h1>
    <h1>{{ abc }}</h1>
    <h2>Essential Links</h2>


    <p v-cloak> ++++++++++{{abc}}+++++++++++</p>
    <div v-text="msg1">  </div>
    <br>
    <div v-html="msg1">  </div>

    <br>
    {{msg1}}
    <br>

    <input type="button" value="按钮"  v-on:click="show" >

    <br>

    <div id="app">
    <p>{{ message }}</p>
    <input type="text" v-model="message"/>
</div>

    <ul>
      <li><a href="https://vuejs.org" target="_blank">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank">Twitter</a></li>
    </ul>
    <h2>Ecosystem</h2>
    <ul>
      <li><a href="http://router.vuejs.org/" target="_blank">vue-router</a></li>
      <li><a href="http://vuex.vuejs.org/" target="_blank">vuex</a></li>
      <li><a href="http://vue-loader.vuejs.org/" target="_blank">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank">awesome-vue</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      abc: 'Welcome to Your itgoyo App',
      msg1: '<h1>Welcome to Your itgoyo App</h1>',
      mytitle: '<h1>Welcome to Your itgoyo App</h1>'
      ,
      methods: {
      show :function(){
        alert("hello")
      }
      }
    }
  }


  // var vm = new Vue({

  //     el: '#app',
  //     data:{
  //     msg: 'Welcome to Your Vue.js App',
  //     abc: 'Welcome to Your itgoyo App',
  //     msg1: '<h1>Welcome to Your itgoyo App</h1>',
  //     mytitle: '<h1>Welcome to Your itgoyo App</h1>'
  //     }
  // })
}
</script>

k<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

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

<template>
  <div id="app">
    <img src="./assets/logo.png">

     <a-button type="primary">Button></a-button>
    <router-link to="/">home</router-link>
    <button @click="go()">点我跳转</button>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'App',
  methods: {
    go () {
      this.$router.push('/home')
    }
  }
}

</script>
<style>

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>

<template>
  <div id="app" @click="test">{{ message }} <router-view /></div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      message: 'Hello commander!'
    }
  },
  methods: {
    test (e) {
      this.message = '123'
      console.log(e)
    }
  }
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

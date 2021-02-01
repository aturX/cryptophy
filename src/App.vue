<template>
  <div id="app">
    <h1></h1>
    <Home :msg="posts"/>
  </div>
</template>

<script>
import Home from './components/Home.vue'

export default {
  name: 'app',
  data: function () {
    return {
      posts: [ 
        { id: 1, text: '测试文本1' },
        { id: 2, text: '测试文本2' },
        { id: 3, text: '测试文本3' }
      ]
    }
  },
  components: {
    Home
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

h1 {
    font-size:64px;
    font-family: Simsun;
    font-weight: normal;
    line-height:1;
    text-shadow:0 3px 0 rgba(0,0,0,0.1);
}

img {
  width:15%;
  height:15%;
  border-radius: 50%;
}
</style>

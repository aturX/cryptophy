<template>
  <div id="app">
    <h1 id="title">币圈哲学</h1>
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
        { id: 1, text: '答应我，赌下去。' },
        { id: 2, text: '白皮书说了，不做事只拉盘。' },
        { id: 3, text: '作为一个炒币者，你买了一个币，却不去传销它，是很不应该的。' },
        { id: 4, text: '放心赌，输了有政府补贴。' },
        { id: 5, text: '你们玩吧，我没钱了。' },
        { id: 6, text: '以前我炒币的时候，只有下跌才会亏钱。后来学习了合约，上涨和下跌都会亏钱。再后来我加强了学习，学会了期权，这下好了，价格不动也会亏钱。' },
        { id: 7, text: '拉盘的事就拜托了。' },
        { id: 8, text: '直接打钱不要问，不要问直接打钱。' },
        { id: 9, text: '分析尼玛，直接说梭哪边。' },
        { id: 10, text: '亲，这边的建议是先充八万呢' }
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

#title {
    font-size:40px;
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

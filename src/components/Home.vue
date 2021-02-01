<template>
  <div class="hello">
    <div id="box">
      <h1>
        {{ getRandom() }}
        </h1>
    </div>
    
 
  </div>
</template>

<script>
export default {
  name: 'Home',
  data: function(){
    return {
      num: 0
    }
  },
  props: {
    msg: Array
  },
  created: function(){
    this.getRandom()
  },
  methods: {
    getRandomInt: function(max) {
      return Math.floor(Math.random() * Math.floor(max));
    },
    getRandom: function() {
      var items = this.msg
      this.num = this.getRandomInt(this.msg.length)
      return items[this.num].text
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  margin: 40px 0 0;
  color: #42b983;
  letter-spacing:1rem;
  font-family: Simsun;
}
 
</style>

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
  color: #358f66;
  letter-spacing:1rem;
  font-family: Simsun;
  font-weight: bold;
  line-height:1;
  text-shadow:0 3px 0 rgba(0,0,0,0.1);
}

#box {
  width: 80%;
  height: 100%;
  margin: 0 auto;
}
 
</style>

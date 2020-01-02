<template>
  <div class="hello">
    <img style="width: 100%" src="./img/01.png" alt="">
    <div class="code" @click="open">沪ICP备19026161号-1</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
    open () {
      window.open('http://www.beian.miit.gov.cn')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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

  .code a {
    font-size: 14px;
    line-height: 40px;
    color: #666666;
  }
</style>

<template>
  <div class="hello">
    <img style="width: 100%" src="./img/01.png" alt="">
    <div class="code" @click="open">沪ICP备19026161号-1</div>
    <div class="code" @click="open2">隐私声明</div>
    <div class="yinsi">
    </div>
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
    open2 () {
      this.$router.push({path: '/ys'})
    },
    open () {
      window.open('http://www.beian.miit.gov.cn')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .yinsi {
    position: fixed;
    left: 50%;
    top: 50%;
    height: 100px;
    width: 100px;
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
  .code {
    cursor: pointer;
    font-size: 14px;
    line-height: 40px;
    color: #666666;
  }
</style>

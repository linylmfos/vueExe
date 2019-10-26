<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <p>$attrs--继承所有的父组件属性（除了prop传递的属性、class 和 style ）</p>
    <HelloWorld msg="Welcome to Your Vue.js App"  mysel="self shu xing" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  },
  mounted() {
    /* eslint-disable */
    console.log('attrs属性', this.$attrs)
    console.log('children', this.$children)
    console.log('parent', this.$parent)
    /* eslint-enable */
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

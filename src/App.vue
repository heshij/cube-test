<template>
  <div id="app">
    <button-test></button-test>
  </div>
</template>

<script>
  import ButtonTest from './components/button-test/button-test'

  export default {
    name: 'app',
    components: {
      ButtonTest
    }
  }
</script>
<style lang="stylus">
  #app
    font-family 'Avenir', Helvetica, Arial, sans-serif
    -webkit-font-smoothing antialiased
    -moz-osx-font-smoothing grayscale
    text-align center
    color #2c3e50
    margin-top 60px
</style>

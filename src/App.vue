<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
  export default {
    name: 'App'
  }
</script>

<style lang="scss">
  @import '~styles/app.scss';

  *{
    box-sizing: border-box;
  }

  body,html {
    height: 100%;
  }

  body{
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    margin: 0;
    background: #21E6C1;
    background: linear-gradient(to left, #21E6C1, #3B2C85);
  }

  #app {
    height: 100%;
  }
</style>

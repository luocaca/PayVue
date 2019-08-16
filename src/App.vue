<template>
  <div id="app">
    <p>
      快速充值
    </p>
    <router-view/>
  </div>
</template>

<script>
  export default {
    name: 'App',

  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;

  }


  input::-webkit-input-placeholder {
    color: #cccccc;
  }

  input::-moz-placeholder { /* Mozilla Firefox 19+ */
    color: #cccccc;
  }

  input:-moz-placeholder { /* Mozilla Firefox 4 to 18 */
    color: #cccccc;
  }

  input:-ms-input-placeholder { /* Internet Explorer 10-11 */
    color: #cccccc;
  }


  /* margin-top: 60px;*/

  p {
    background: #23b5e2;
    margin: 0;
    color: white;
    max-width: 1080px;
    padding: 10px;
    width: 100%;

  }

  body{
    margin:0;
    padding:0;
  }

</style>

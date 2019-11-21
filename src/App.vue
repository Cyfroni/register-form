<template>
  <div id="app">
    <Register />
  </div>
</template>

<script>
import Register from './views/Register'

export default {
  name: 'app',
  components: {
    Register
  }
}
</script>

<style>
#app {
  background-image: url('./assets/background.jpg');
  background-position: right;
  background-size: cover;
  min-height: 100vh;
}
.wedio-white {
  color: white;
}
</style>

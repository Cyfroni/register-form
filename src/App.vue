<template>
  <div id="app" style>
    <RegisterForm />
  </div>
</template>

<script>
import RegisterForm from './components/RegisterForm.vue'

export default {
  name: 'app',
  components: {
    RegisterForm
  }
}
</script>

<style>
#app {
  background-image: url('https://wedio-cdn.s3.eu-west-1.amazonaws.com/images/homepage/login/login_bg_x3.jpg');
  background-position: right;
  background-size: cover;

  min-height: 100vh;
  position: relative;
}
</style>

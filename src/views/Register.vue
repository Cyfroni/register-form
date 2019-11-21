<template>
  <div class="register">
    <h1 class="wedio-white">WELCOME TO WEDIO -</h1>
    <p class="wedio-white">
      the fastest-growing European community of creators
    </p>
    <RegisterForm />
  </div>
</template>

<script>
import RegisterForm from '../components/RegisterForm'

export default {
  name: 'register',
  components: {
    RegisterForm
  }
}
</script>

<style scoped>
.register {
  width: 450px;
  position: absolute;
  top: 50%;
  left: 30%;
  transform: translate(-50%, -50%);
}
</style>

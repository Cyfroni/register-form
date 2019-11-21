<template>
  <div class="registerForm">
    <Form
      inputId="EmailInput"
      name="Email"
      type="email"
      placeholder="Enter email"
    />
    <Form
      inputId="UsernameInput"
      name="Username"
      type="email"
      placeholder="Enter username"
    />
    <Form
      inputId="PasswordInput"
      name="Password"
      type="password"
      placeholder="Enter password"
    />
    <p id="termsAndConditions" class="wedio-white">
      <span>
        By clicking on Register, you agree to Wedio's
        <a
          class="wedio-white"
          href="http://support.wedio.com/en/articles/3491417-terms-and-conditions"
          >Terms & Conditions</a
        >
        and
        <a
          class="wedio-white"
          href="http://support.wedio.com/en/articles/3491350-privacy-policy-your-data-your-decision"
          >Privacy Policy</a
        >.
      </span>
    </p>
    <div>
      <button type="button" class="btn btn-outline-light">SIGN IN</button>
      <button type="button" class="btn btn-success" @click="doSubmit">
        REGISTER
      </button>
    </div>
  </div>
</template>

<script>
import Form from './common/Form'
export default {
  name: 'RegisterForm',
  components: {
    Form
  },
  methods: {
    doSubmit() {
      console.log(this.input)
    }
  }
}
</script>

<style scoped>
.btn {
  margin: 10px 30px 10px 30px;
  border-radius: 30px;
  width: 150px;
}
a {
  text-decoration: underline;
}
</style>

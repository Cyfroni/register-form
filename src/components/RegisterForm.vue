<template>
  <form>
    <h1>WELCOME TO WEDIO -</h1>
    <p>the fastest-growing European community of creators</p>
    <div class="form-group">
      <label for="EmailInput">Email</label>
      <input
        v-model="input.email"
        type="email"
        class="form-control"
        id="EmailInput"
        placeholder="Enter email"
      />
    </div>
    <div class="form-group">
      <label for="UsernameInput">Username</label>
      <input
        v-model="input.username"
        type="email"
        class="form-control"
        id="UsernameInput"
        placeholder="Enter username"
      />
    </div>
    <div class="form-group">
      <label for="InputPassword">Password</label>
      <input
        v-model="input.password"
        type="password"
        class="form-control"
        id="InputPassword"
        placeholder="Enter password"
      />
    </div>
    <p id="emailHelp" class="form-text text-muted">
      By clicking on Register, you agree to Wedio's Terms & Conditions and
      Privacy Policy..
    </p>
    <button type="button" class="btn btn-outline-light">SIGN IN</button>
    <button type="button" class="btn btn-success" @click="register()">
      REGISTER
    </button>
  </form>
</template>

<script>
export default {
  name: 'RegisterForm',
  data() {
    return { input: { email: '', username: '', password: '' } }
  },
  methods: {
    register() {
      console.log(this.input)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.btn {
  margin: 10px 30px 10px 30px;
  border-radius: 30px;
  width: 150px;
}

form {
  width: 450px;
  position: absolute;
  top: 50%;
  left: 30%;
  transform: translate(-50%, -50%);
}
</style>

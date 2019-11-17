<template>
  <form>
    <h1>WELCOME TO WEDIO -</h1>
    <p>the fastest-growing European community of creators</p>
    <div class="form-group">
      <label for="EmailInput">Email</label>
      <input
        type="email"
        class="form-control"
        id="EmailInput"
        placeholder="Enter email"
      />
    </div>
    <div class="form-group">
      <label for="UsernameInput">Username</label>
      <input
        type="email"
        class="form-control"
        id="UsernameInput"
        placeholder="Enter username"
      />
    </div>
    <div class="form-group">
      <label for="InputPassword">Password</label>
      <input
        type="password"
        class="form-control"
        id="InputPassword"
        placeholder="Enter password"
      />
    </div>
    <small id="emailHelp" class="form-text text-muted"
      >By clicking on Register, you agree to Wedio's Terms & Conditions and
      Privacy Policy..</small
    >
    <button type="button" class="btn btn-primary">
      REGISTER
    </button>
    <button type="button" class="btn btn-outline-primary">
      SIGN IN
    </button>
  </form>
</template>

<script>
export default {
  name: 'RegisterForm'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.btn {
  margin: 50px;
  border-radius: 30px !important;
}

form {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>

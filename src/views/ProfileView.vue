<template>
  <div class="container">
    <div class="form">
      <h2>Login</h2>
      <form @submit.prevent="login">
        <div>
          <label>Email:</label>
          <input type="email" v-model="loginForm.email" required />
        </div>
        <div>
          <label>Password:</label>
          <input type="password" v-model="loginForm.password" required />
        </div>
        <button type="submit">Login</button>
      </form>
    </div>
    <div class="form2">
      <h2>Register</h2>
      <form @submit.prevent="register">
        <div>
          <label>Name:</label>
          <input type="text" v-model="registerForm.name" required />
        </div>
        <div>
          <label>Email:</label>
          <input type="email" v-model="registerForm.email" required />
        </div>
        <div>
          <label>Password:</label>
          <input type="password" v-model="registerForm.password" required />
        </div>
        <div>
          <label>Confirm Password:</label>
          <input
            type="password"
            v-model="registerForm.confirmPassword"
            required
          />
        </div>
        <button type="submit">Register</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "LoginForm",
  data() {
    return {
      loginForm: {
        email: "",
        password: "",
      },
      registerForm: {
        name: "",
        email: "",
        password: "",
        confirmPassword: "",
      },
    };
  },
  methods: {
    login() {
      // Handle login logic
      console.log(this.loginForm);
      this.loginForm.email = "";
      this.loginForm.password = "";
    },
    register() {
      // Handle registration logic
      console.log(this.registerForm);
      this.registerForm.name = "";
      this.registerForm.email = "";
      this.registerForm.password = "";
      this.registerForm.confirmPassword = "";
    },
  },
};
</script>

<style scoped>

.container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: baseline;
  
}

.form2 {
  width: 50%;
  height: 100vh;
  background-color: rgb(215, 213, 213);
}
.form {
  display: flex;
  flex-direction: column;
  width: 25%;
  height: 100vh;

}

div {
  margin-bottom: 10px;
}

label {
  font-weight: bold;
  display: block;
  margin-bottom: 5px;
}

input {
  padding: 5px;
  border-radius: 5px;
  border: 1px solid #ccc;
}

button {
  padding: 5px 10px;
  background-color: #ff8400;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}
</style>

<template>
  <div id="login" class="text-center">
    <form class="form-signin" @submit.prevent="login">
      <section class="hero is-success is-small"> 
  <div class="hero-body">
    <div class="container">
      <h1 class="title">
        Sign In To Your Account
      </h1>
      
    </div>
  </div>
</section>
      
      <div
        class="alert alert-danger"
        role="alert"
        v-if="invalidCredentials"
      >Invalid username and password!</div>
     
      <div
        class="alert alert-success"
        role="alert"
        v-if="this.$route.query.registration"
      >Thank you for registering, please sign in.</div>
     
      <div class="field column is-one-third is-centered">
        <p class="control">
          <label for="username" class="label">Username</label>
          <input
            type="text"
            id="username"
            class="input"
            placeholder="Username"
            v-model="user.username"
            required
            autofocus
          />
        </p>
        <p class="control">
          <label for="password" class="label">Password</label>
          <input
            type="password"
            id="password"
            class="input"
            placeholder="Password"
            v-model="user.password"
            required
          />
        
        </p>

        <button type="submit" class="button is-success">Sign in</button>
        <br />
         <!-- <router-link :to="{ name: 'register' }">Need an account? Click here to register.</router-link> -->
      </div>
    </form>
  </div>
  
</template>

<script>
import auth from "../auth";

export default {
  name: "login",
  components: {},
  data() {
    return {
      user: {
        username: "",
        password: ""
      },
      invalidCredentials: false
    };
  },
  methods: {
    login() {
      fetch(`${process.env.VUE_APP_REMOTE_API}/login`, {
        method: "POST",
        headers: {
          Accept: "application/json",
          "Content-Type": "application/json"
        },
        body: JSON.stringify(this.user)
      })
        .then(response => {
          if (response.ok) {
            return response.text();
          } else {
            this.invalidCredentials = true;
          }
        })
        .then(token => {
          if (token != undefined) {
            if (token.includes('"')) {
              token = token.replace(/"/g, "");
            }
            auth.saveToken(token);
            this.$emit('logInEvent');
            this.$router.push("/");
          }
        })
        .catch(err => console.error(err));
    }
  }
};
</script>

<style>
@import 'https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css';
</style>

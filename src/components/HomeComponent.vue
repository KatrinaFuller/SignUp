<template>
  <div class="row homeComponent">
    <div class="col-12">
      <h1>My Wishlist</h1>
    </div>
    <div class="col-6">
      <!-- Login -->
      <form v-if="loginForm" @submit.prevent="loginUser">
        <div class="form-group">
          <input type="email" v-model="creds.email" placeholder="Email" />
        </div>
        <div class="form-group">
          <input type="password" v-model="creds.password" placeholder="Password" />
        </div>
        <button type="submit" class="btn btn-primary m-2">Login</button>
      </form>

      <!-- Sign Up -->
      <form v-else @submit.prevent="register">
        <div class="form-group">
          <input type="text" v-model="newUser.name" placeholder="Name" />
        </div>
        <div class="form-group">
          <input type="email" v-model="newUser.email" placeholder="Email" />
        </div>
        <div class="form-group">
          <input type="password" v-model="newUser.password" placeholder="Password" />
        </div>
        <button type="submit" class="btn btn-primary">Register</button>
      </form>

      <div class="action text" @click="loginForm = !loginForm">
        <p v-if="loginForm">No account? Click here to Register</p>
        <p v-else>Already have an account? Click here to Login</p>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "homeComponent",
  data() {
    return {
      loginForm: true,
      creds: {
        email: "",
        password: ""
      },
      newUser: {
        email: "",
        password: "",
        name: ""
      }
    };
  },
  // beforeCreate() {
  //   if (this.$store.state.user._id) {
  //     this.$router.push({ name: "home" });
  //   }
  // },
  computed: {},
  methods: {
    // register() {
    //   this.$store.dispatch("register", this.newUser);
    // },
    // loginUser() {
    //   this.$store.dispatch("login", this.creds);
    // }
  },
  components: {}
};
</script>


<style scoped>
</style>
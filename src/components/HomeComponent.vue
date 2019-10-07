<template>
  <div class="row homeComponent">
    <div class="col-12">
      <h1>My Wishlist</h1>
    </div>
    <div class="col-6">
      <form>
        <div class="form-group">
          <!-- <label for="email">Email address</label> -->
          <input type="email" class="form-control" id="email" placeholder="Email" />
        </div>
        <div class="form-group">
          <!-- <label for="password">Password</label> -->
          <input type="password" class="form-control" id="password" placeholder="Password" />
        </div>
        <button type="submit" class="btn btn-primary m-2">Login</button>
        <button type="submit" class="btn btn-primary">Register</button>
      </form>
    </div>
  </div>
</template>


<script>
export default {
  name: "homeComponent",
  data() {
    return {};
  },
  computed: {},
  methods: {},
  components: {}
};
</script>


<style scoped>
</style>
<template>
  <div class="home container-fluid">
    <HomeComponent />
  </div>
</template>

<script>
// @ is an alias to /src
import HomeComponent from "../components/HomeComponent";

export default {
  name: "home",
  components: {
    HomeComponent
  }
};
</script>

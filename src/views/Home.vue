<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <div><home /></div>
  </div>
</template>

<script>
import home from "../components/homecomponents.vue";
import store from "@/store.js";
export default {
  name: "Home",
  components: {
    home,
  },
  data() {
    return {
      destination: store.destination,
    };
  },
};
</script>

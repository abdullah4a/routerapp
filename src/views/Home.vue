<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <div><home /></div>
    <div><Boosatrap /></div>
  </div>
</template>

<script>
import home from "../components/homecomponents.vue";
import Boosatrap from "../components/boosatrap.vue";
import store from "../store.js";
export default {
  name: "Home",
  components: {
    home,
    Boosatrap,
  },
  data() {
    return {
      destination: store.destination,
    };
  },
};
</script>

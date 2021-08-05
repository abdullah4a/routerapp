<template>
  <div id="home">
    <div class="container-fluid">
      <h1>First Responsive app</h1>
      <p>Resize the browser window to see the effect.</p>

      <div class="row nav justify-content-center">
        <div
          class="col-lg-4"
          style="background-color: ; margin: 10px"
          v-for="imag in images"
          :key="imag"
        >
          <img
            :src="imag"
            style="width: 100%; max-width: 400px; max-height: 300px"
          />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import image from "E:/abdullah/RouterApp/routerapp/src/assets/1.jpg";
import image1 from "E:/abdullah/RouterApp/routerapp/src/assets/2.jpg";
import image2 from "E:/abdullah/RouterApp/routerapp/src/assets/3.jpg";
import image3 from "E:/abdullah/RouterApp/routerapp/src/assets/4.jpg";
import image4 from "E:/abdullah/RouterApp/routerapp/src/assets/Plants.jpg";
import image5 from "E:/abdullah/RouterApp/routerapp/src/assets/mia.jpg";
import image6 from "E:/abdullah/RouterApp/routerapp/src/assets/Frozen.jpg";
import image7 from "E:/abdullah/RouterApp/routerapp/src/assets/Eyes.jpg";
import image8 from "E:/abdullah/RouterApp/routerapp/src/assets/Burns.jpg";

export default {
  data() {
    return {
      images: [
        image,
        image1,
        image2,
        image3,
        image4,
        image5,
        image6,
        image7,
        image8,
      ],
      showdes: false,
    };
  },
  methods: {
    Isactive() {
      return true;
    },
  },
};
</script>
<style>
.brandimage {
  width: 400px;
  height: 200px;
  padding: 2px;
  display: inline-block;
  margin: 0px 50px;
  border: 1px solid red;
}
.brandimage img {
  width: 400px;
  height: 200px;
}
.nav-bar {
  float: left;
  margin: 5px 10px;
  width: 28%;
  height: 500px;
  border: 1px dotted gray;
}
.newsfeed {
  display: inline-block;
  margin: 0px 10px;
  width: 68%;
  border: 1px solid rgb(111, 114, 111);
}
@import "~bootstrap/dist/css/bootstrap.css";
</style>

<template lang="HTML">
  <div>
    <div class="container-fluid">
      <h1>Hello World!</h1>
      <p>Resize the browser window to see the effect.</p>
      <p>
        The columns will automatically stack on top of each other when the
        screen is less than 768px wide.
      </p>
      <div class="row">
        <div class=""
      </div>
    </div>
  </div>
</template>
>
<!-- <div class="home container-fluid">
    <div class="nav-bar">
      <h1>This is Nav Header</h1>
      <p>This is Nav buttons Bar</p>
    </div>
    <div class="list-inline">
      <div id="container-fluid">
        this is News Feeds upper bar <code>span</code>
      </div>
      <div class="row">
        <div class="brandimage">
          <div
            class="col-sm-4"
            style="background-color: lavender"
            v-for="imag in image"
            :key="imag"
          >
            <img :src="imag" />
          </div>
          <input type="checkbox" v-model="showdes" />
          <div class="" v-if="showdes">This image is an Hd Walpaper</div>
        </div>
      </div>
    </div>
  </div> 
</template>-->
<script>
import image from "E:/abdullah/RouterApp/routerapp/src/assets/1.jpg";
import image1 from "E:/abdullah/RouterApp/routerapp/src/assets/2.jpg";
import image2 from "E:/abdullah/RouterApp/routerapp/src/assets/3.jpg";
import image3 from "E:/abdullah/RouterApp/routerapp/src/assets/4.jpg";

export default {
  data() {
    return {
      images: [image, image1, image2, image3],
      showdes: false,
    };
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

<template>
  <div class="home">
    <div class="nav-bar">
      <h1>This is Nav Header</h1>
      <p>This is Nav buttons Bar</p>
    </div>
    <div class="newsfeed">
      <div id="newsfeed-upperbar">this is News Feeds upper bar</div>
      <!-- <div class="destination">
        <div v-for="dest in destination" :key="dest.name">
          <router-link :to="dest.slug">
            <h2>{{ dest.name }}</h2>
          </router-link>
          <figure>
            <router-link :to="dest.name">
              <img :src="require(`@/assets/${dest.image}`)" :alt="dest.name" />
            </router-link>
          </figure>
        </div>
      </div> -->
      <div class="brandimage" v-for="imag in image" :key="imag">
        <img :src="imag" />
        <input type="checkbox" v-model="showdes" />
        <div class="" v-if="showdes">This image is an Hd Walpaper</div>
      </div>
    </div>
  </div>
</template>
<script>
import image from "E:/abdullah/RouterApp/routerapp/src/assets/1.jpg";
import image1 from "E:/abdullah/RouterApp/routerapp/src/assets/2.jpg";
import image2 from "E:/abdullah/RouterApp/routerapp/src/assets/3.jpg";
import image3 from "E:/abdullah/RouterApp/routerapp/src/assets/Mia.png";

export default {
  data() {
    return {
      image: [image, image1, image2, image3],
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
  margin: 10px 50px;
  border: 1px solid red;
}
.brandimage img {
  width: 400px;
  height: 200px;
}
.nav-bar {
  margin: 5px 10px;
  width: 28%;
  height: 500px;
  border: 1px dotted gray;
  display: inline-block;
}
.newsfeed {
  float: right;
  margin: 5px 10px;
  width: 68%;
  height: 500 px;
  border: 1px solid green;
}
</style>

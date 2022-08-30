<template>
  <div>
    <el-carousel type="card" height="700px" width="400px" >
      <el-carousel-item v-for="item in flowerPics" :key="item" autoplay>
       <img :src="item" style="width:100%; height:100%"/>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<script>
import img1 from "./assets/image1.jpg";
import img2 from "./assets/image2.jpg";
import img3 from "./assets/flower3.jpg";
import img4 from "./assets/flower4.jpeg";
import img5 from "./assets/flower5.jpg";
import img6 from "./assets/flower6.jpg";

export default {
  name: "App",

  components: {},
  data() {
    return {
      img1,
      flowerPics: [img1, img2, img3, img4, img5, img6],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.el-carousel__item h3 {
  color: #475669;
  opacity: 0.75;
  line-height: 200px;
  margin: 0;
  text-align: center;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
</style>
<template>
  <div>
    <!-- directive -->
    <!-- <div class="images" v-viewer>
      ALGUM TEXTO
      <img v-for="src in images" :key="src" :src="src" />
    </div> -->

    <!-- <div class="images" v-viewer>    
      <img v-for="src in images" :key="src" :src="src" />
    </div> -->
    <!-- component -->
    <input type="text" v-model="qqrcoisa.name">
    {{qqrcoisa.name}}
    <viewer :images="images">
      <div v-for="src in images" :key="src.img" >
        <img :src="src.img" />
        <div>
          <label for="">{{src.txt}}</label>
        </div>
      </div>
      <!-- <img v-for="src in images" :key="src.img" :src="src.img" /> -->
    </viewer>
    <!-- api -->
    <button type="button" @click="show">Click to show</button>
  </div>
</template>
<script>
import "viewerjs/dist/viewer.css";
import VueViewer from "v-viewer";
import Vue from "vue";
Vue.use(VueViewer);
export default {
  data() {
    return {
      images: [
        // { img: "https://picsum.photos/200/200", txt: "acs" },
        // { img: "https://picsum.photos/300/200", txt: "me myself" },
        // { img: "https://picsum.photos/250/250", txt: "bacurau" },
      ],
      qqrcoisa:{
        name:''
      }
    };
  },
  methods: {
    show() {
      this.$viewerApi({
        images: this.images,
      });
    },
  },
};
</script>
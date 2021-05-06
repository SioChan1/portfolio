<template>
  <v-row>
    <!-- Start Blog Area  -->
    <v-col
      lg="4"
      md="4"
      sm="6"
      cols="12"
      v-for="(item, i) in blogContent"
      :key="i"
    >
      <div class="blog blog-style--1">
        <div class="thumbnail">
          <p>
            <img class="w-100" :src="item.src" alt="Blog Images" />
          </p>
        </div>
        <div class="content">
          <p class="blogtype">{{ item.meta }}</p>
          <h4 class="heading-title">
            <p>{{ item.title }}</p>
          </h4>
          
        </div>
      </div>
    </v-col>
    <!-- End Blog Area  -->
  </v-row>
</template>

<script>
  export default {
    data() {
      return {
        blogContent: [
          {
            src: require("../../assets/images/blog/blog-01.jpg"),
            meta: "",
            title: "E-style girl",
          },
          {
            src: require("../../assets/images/blog/blog-02.jpg"),
            meta: "",
            title: "Street lights",
          },
          {
            src: require("../../assets/images/blog/blog-03.jpg"),
            meta: "",
            title: "The look",
          },
        ],
      };
    },
  };
</script>

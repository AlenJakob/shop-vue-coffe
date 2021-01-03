<template>
  <b-carousel :pause-info="false" class="carousel" :indicator-inside="true">
    <b-carousel-item v-for="(item, i) in 3" :key="i">
      <span class="image">
        <img :src="getImgUrl(i)" />
      </span>
    </b-carousel-item>
  </b-carousel>
</template>

<script>
export default {
  methods: {
    getImgUrl(value) {
      let arr = [
        "https://images.pexels.com/photos/585750/pexels-photo-585750.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
        "https://images.pexels.com/photos/894695/pexels-photo-894695.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
        "https://images.pexels.com/photos/324028/pexels-photo-324028.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
      ];
      return arr[value];
    },
  },
};
</script>

<style>
.is-active .al img {
  filter: grayscale(0%);
}
.al img {
  filter: grayscale(100%);
}
.carousel .carousel-items .carousel-item {
  max-height: 600px;
}
</style>
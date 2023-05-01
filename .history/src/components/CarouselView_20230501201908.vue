<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->
      <b-carousel-slide
        caption="First slide"
        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
        img-src="https://asset.kompas.com/crops/V6ViT5zjwooMiYHjl922Cl5FMOM=/0x0:0x0/750x500/data/photo/2022/06/29/62bc3c5f26d8d.jpg"
      ></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide
        img-src="https://cdn0-production-images-kly.akamaized.net/Jd7Y8kbKB4JcGT_8Dm1FpZ1uJd4=/1200x675/smart/filters:quality(75):strip_icc():format(jpeg)/kly-media-production/medias/1229890/original/049959100_1462958790-18th-amendment-barbershop-gastown-3.jpg"
      >
        <h1>Hello world!</h1>
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide
        img-src="https://www.masterseo.id/wp-content/uploads/2020/02/barbershop-medan-840x450.jpg"
      ></b-carousel-slide>

      <!-- Slides with img slot -->
      <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
      <b-carousel-slide>
        <template #img>
          <img
            class="d-block img-fluid w-100"
            width="1024"
            height="480"
            src="https://cdn1-production-images-kly.akamaized.net/UhHYLrUThWl7vzCRrVu6WQ5STp8=/1200x900/smart/filters:quality(75):strip_icc():format(jpeg)/kly-media-production/medias/4100221/original/015056800_1658739577-pexels-thgusstavo-santana-1813272_1_.jpg"
            alt="image slot"
          />
        </template>
      </b-carousel-slide>
    </b-carousel>
  </div>
</template>

<script>
export default {
  name: "CarouselView",
  data() {
    return {
      slide: 0,
      sliding: null,
    };
  },
  methods: {
    onSlideStart() {
      this.sliding = true;
    },
    onSlideEnd() {
      this.sliding = false;
    },
  },
};
</script>
<template>
  <div class="home mt-5 pt-2">
    <div class="row">
      <div class="col">
        <carousel-view />
      </div>
    </div>
  </div>
</template>

<script>
import CarouselView from "@/components/CarouselView.vue";

export default {
  name: "HomeView",
  components: { CarouselView },
};
</script>

    CarouselView
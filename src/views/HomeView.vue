<template>
  <div class="home mt-5 pt-2">
    <div class="row">
      <div class="col-12">
        <carousel-view />
      </div>
      <div class="col-12 text-warning text-center mt-3">
        <h1 class="p-1">Tentang <strong>Barbershop</strong></h1>
        <p class="p-3">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat,
          libero quos! Voluptas dolorum sunt voluptate quibusdam doloribus.
          Fugiat obcaecati impedit quod itaque? Dolores obcaecati quaerat
          facilis alias distinctio dignissimos, maiores laborum asperiores sit
          enim rerum quam tempora eum, voluptatum iste dolor perferendis, rem
          beatae minima porro ducimus maxime! Consequuntur, tenetur!
        </p>
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
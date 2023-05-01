<template>
  <div class="fixed-top">
    <b-navbar type="dark" variant="dark">
      <router-link class="navbar-brand text-warning" to="/">
        <strong> BarberShop</strong>
      </router-link>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <router-link class="nav-item text-warning" to="/tentang">
            Tentang
          </router-link>
          <router-link class="nav-item text-warning" to="/reservasi">
            Reservasi
          </router-link>
          <router-link class="nav-item text-warning" to="/">
            Galeri
          </router-link>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "NavbarView",
};
</script>

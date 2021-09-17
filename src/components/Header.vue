<template>
  <!-- NAVBAR  -->
  <nav class="navbar position-absolute">
    <div class="container py-4">
      <img :src="logo" alt="avadabarbers-logo-200x70" />
      <div class="cursor">
        <a class="navbar-brand" href="#">
          <i class="fas fa-shopping-cart fs-5 ms-1"></i>
        </a>
        <a class="navbar-brand" href="#">
          <i class="fas fa-bars fs-5 ms-1"></i>
        </a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Header",
  props: ["logo"],
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";

.navbar {
  width: 100%;
}
a {
  color: $popular;
  &:hover {
    color: $important;
  }
}
</style>

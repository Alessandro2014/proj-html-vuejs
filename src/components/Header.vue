<template>
    <!-- NAVBAR  -->
    <nav class="navbar position-absolute">
      <div class="container py-4">
        <img
          src="@/assets/img/avadabarbers-logo-200x70.png"
          alt="logo"
          class="img-fluid"
        />
        <div class="cursor">
          <a class="navbar-brand" href="#">
            <i class="fas fa-shopping-cart fs-4 m-1"></i>
          </a>
          <a class="navbar-brand" href="#">
            <i class="fas fa-bars fs-4 m-1"></i>
          </a>
        </div>
      </div>
    </nav>
</template>

<script>
export default {
  name: "Header",
  props: {},
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";

.navbar{
  height: 90px;
  width: 100%;
  a {
    color: $popular;
  }
}
</style>

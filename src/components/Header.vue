<template>
  <div class="hello">
    <!-- NAVBAR  -->
    <nav class="navbar">
      <div class="container py-4">
        <img
          src="@/assets/img/avadabarbers-logo-200x70.png"
          alt="logo"
          class=""
        />
        <div>
          <a class="navbar-brand" href="#">
            <i class="fas fa-shopping-cart fs-4"></i>
          </a>
          <a class="navbar-brand" href="#">
            <i class="fas fa-bars fs-4"></i>
          </a>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Header",
  props: {},
};
</script>

<style scoped lang="scss"></style>

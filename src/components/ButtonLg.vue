<template>
  <div>
    <!-- COMPONENTE BOTTONE IMPORTATO NEGLI ALTRI COMPONENTI -->
    <div
      class="button-avada-large d-inline-block text-uppercase fw-bolder py-3 px-4 my-2"
    >
      <a href="#" class="text-decoration-none ">
        <slot></slot>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "ButtonLg",
};
</script>

<style lang="scss">
@import "../scss/style.scss";
// STILE GLOBALE PER LE A CON CLASSE "button-avada-large"
.button-avada-large {
  border: 2px solid $important;
  a {
    color: $important;
    font-family: $font-general;
  }
}
</style>

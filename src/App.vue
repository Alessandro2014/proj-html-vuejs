<template>
  <div id="app">
    <!-- COMPONENTE HEADER -->
    <Header msg="Inizializzazione progetto" />
  </div>
</template>

<script>
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: {
    Header,
  },
};
</script>

<style lang="scss">
// IMPORTO STYLE CON BOOTSTRAP
@import "scss/style.scss";
</style>

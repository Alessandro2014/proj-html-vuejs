<template>
  <div id="app">
    <!-- COMPONENTE HEADER -->
    <header>
      <Header />
    </header>
    <main>
      <SectionHero
        title="Barber Shop"
        slogan="The Pinnacle of Male Grooming"
        button="LEARN MORE"
      />
    </main>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import SectionHero from "@/components/SectionHero.vue";

export default {
  name: "App",
  components: {
    Header,
    SectionHero,
  },
};
</script>

<style lang="scss">
// IMPORTO STYLE CON BOOTSTRAP
@import "scss/style.scss";
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
</style>

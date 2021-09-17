<template>
  <div id="app">
    <!-- COMPONENTE HEADER -->
    <header>
      <Header :logo="logo" />
    </header>
    <main>
      <Hero
        title="Barber Shop"
        slogan="The Pinnacle of Male Grooming"
      />
      <Main/>
    </main>
    <footer>
      <Footer :logo="logo" />
      <Credits/>
    </footer>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Hero from "@/components/Hero.vue";
import Main from "@/components/Main.vue";
import Footer from "@/components/Footer.vue";
import Credits from "@/components/Credits.vue";


export default {
  name: "App",
  data() {
    return {
      logo: require("@/assets/img/avadabarbers-logo-200x70.png"),
    }
  },
  components: {
    Header,
    Hero,
    Main,
    Footer,
    Credits
  },
};
</script>

<style lang="scss">
// IMPORTO STYLE CON BOOTSTRAP
@import "scss/style.scss";
</style>

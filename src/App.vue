<template>
  <div id="app">
    <!-- COMPONENTE HEADER -->
    <header>
      <Header />
    </header>
    <main>
      <Hero
        title="Barber Shop"
        slogan="The Pinnacle of Male Grooming"
        button="learn more"
      />
      <Main/>
    </main>
    <footer>
      <Footer />
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
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
</style>

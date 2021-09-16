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
        button="learn more"
      />
      <ShoppingCart info="Demos" cart="On Sale" value="39" />
      <SectionAward />
      <SectionServices />
      <SectionProducts />
      <SectionReviews />
      <SectionBlog/>
    </main>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import SectionHero from "@/components/SectionHero.vue";
import ShoppingCart from "@/components/ShoppingCart.vue";
import SectionAward from "@/components/SectionAward.vue";
import SectionServices from "@/components/SectionServices.vue";
import SectionProducts from "@/components/SectionProducts.vue";
import SectionReviews from "@/components/SectionReviews.vue";
import SectionBlog from "@/components/SectionBlog.vue";


export default {
  name: "App",
  components: {
    Header,
    SectionHero,
    ShoppingCart,
    SectionAward,
    SectionServices,
    SectionProducts,
    SectionReviews,
    SectionBlog,
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

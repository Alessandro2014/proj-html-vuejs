<template>
  <main>
    <!-- IMPORTO COMPONENTI RELATIVI AL MAIN -->
    <ShoppingCart info="Demos" cart="On Sale" value="39" />
    <SectionAward />
    <SectionServices />
    <SectionProducts />
    <SectionReviews />
    <SectionBlog />
  </main>
</template>

<script>
import ShoppingCart from "@/components/ShoppingCart.vue";
import SectionAward from "@/components/SectionAward.vue";
import SectionServices from "@/components/SectionServices.vue";
import SectionProducts from "@/components/SectionProducts.vue";
import SectionReviews from "@/components/SectionReviews.vue";
import SectionBlog from "@/components/SectionBlog.vue";

export default {
  name: "Main",
  components: {
    ShoppingCart,
    SectionAward,
    SectionServices,
    SectionProducts,
    SectionReviews,
    SectionBlog,
  },
};
</script>

<style lang="scss"></style>

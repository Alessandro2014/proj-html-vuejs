<template>
  <!-- IMMAGINE PRINCIPALE E TITOLO  -->
  <section id="hero">
    <div class="container">
      <div class="row">
        <!-- COLONNA INFO DI PRESENTAZIONE -->
        <div
          class="col-6 d-flex align-items-start flex-column justify-content-center py-5 d-grid gap-4"
        >
          <h1>{{ title }}</h1>
          <div class="border-separator"></div>
          <h4>{{ slogan }}</h4>
          <ButtonLg class=" button-more">
            learn moore
          </ButtonLg>
        </div>
        <!-- COLONNA FOTO -->
        <div class="col-6">
          <img
            src="@/assets/img/avadabarbers_hero_focalmirror.png"
            alt="avadabarbers-logo-200x70"
            class="img-fluid"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import ButtonLg from "@/components/ButtonLg.vue";
export default {
  name: "SectionHero",
  props: ["title", "slogan"],
  components: {
    ButtonLg,
  },
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";

// BACKGROUND
#hero {
  height: 100vh;
  background-image: url("../assets/img/avadabarbers-hero-bg.jpg");
  background-size: cover;
  background-position: top;
  background-repeat: no-repeat;
}
// COLONNE
.row {
  padding: 100px 0;
}

.border-separator {
  height: 3px;
  width: 250px;
  background-color: $important;
}

h1 {
  font-size: 5.5rem;
  color: $popular;
  font-family: $font-avada;
}

h4 {
  font-size: 1.5rem;
  font-family: $font-general;
  color: $regular;
  font-weight: 400;
}

//BOTTONE

.button-more:hover {
  background-color: black;
}
</style>

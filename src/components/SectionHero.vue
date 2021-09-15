<template>
  <!-- IMMAGINE PRINCIPALE E TITOLO  -->
  <section id="hero">
    <div class="container">
      <div class="row">
        <!-- COLONNA INFO DI PRESENTAZIONE -->
        <div
          class="col-6 d-flex align-items-start flex-column justify-content-center py-5 d-grid gap-5"
        >
          <h1>{{ title }}</h1>
          <div class="border-separator"></div>
          <h3>{{ slogan }}</h3>
          <div>
            <a href="">{{ button }}</a>
          </div>
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
export default {
  name: "SectionHero",
  props: ["title", "slogan", "button"],
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";

#hero {
  height: 100vh;
  background-image: url("../assets/img/avadabarbers-hero-bg.jpg");
}

.row {
  padding: 100px 0;
}

.border-separator {
  height: 3px;
  width: 200px;
  background-color: $important;
}

h1 {
  font-size: 4rem;
  color: $popular;
}

h3 {
  font-size: 1.5rem;
}
</style>

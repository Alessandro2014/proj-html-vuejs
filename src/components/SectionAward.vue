<template>
  <!-- IMMAGINE BACKGROUND  -->
  <section id="awards" class="  position-relative">
    <div class="container">
      <!-- COLONNA INFO DI PRESENTAZIONE -->
      <div
        class="
          content-award
          col-12
          d-flex
          align-items-center
          flex-column
          justify-content-center
          py-5
          d-grid
          gap-2
        "
      >
        <h4>AWARD WINNING</h4>
        <h2>Pro Barbers</h2>
        <ButtonLg>
          meet your new barber
        </ButtonLg>
      </div>
    </div>
    <!-- SEPARATORE CON SVG -->
    <div class="separator">
      <svg
        class="fusion-big-triangle-candy position-absolute"
        xmlns="http://www.w3.org/2000/svg"
        version="1.1"
        width="100%"
        height="100"
        viewBox="0 0 100 100"
        preserveAspectRatio="none"
        style="fill:#fcfcfc;padding:0;"
      >
        <path d="M0 100 L50 2 L100 100 Z" />
      </svg>
    </div>
  </section>
</template>

<script>
import ButtonLg from "@/components/ButtonLg.vue";
export default {
  name: "SectionAward",
  components: {
    ButtonLg,
  },
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";
// IMMAGINE BACKGROUND
#awards {
  height: 550px;
  background-image: url("../assets/img/avadabarbers-introbackground.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: top;
}

.content-award {
  height: 450px;
}

// TESTO
h2 {
  font-size: 4.5rem;
  color: $title;
  font-family: $font-avada;
}

h4 {
  font-size: 1.1rem;
  font-family: $font-general;
  color: $important;
  font-weight: 400;
}

//POSIZIONAMENTO SVG
svg {
  bottom: 0;
  left: 0;
}
</style>

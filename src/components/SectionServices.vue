<template>
  <!-- SEZIONE  SERVICES-->
  <section id="services" class="position-relative">
    <div class="container">
      <!-- COLONNA TITOLO -->
      <div class="row text-center">
        <div class="col-12">
          <h4>MENS GROOMING</h4>
        </div>
        <div class="col-12 pb-5">
          <h2>Services</h2>
        </div>
        <!-- COLONNE DESCRIZIONE SERVIZI -->
        <div class="col-4 p-5">
          <figure>
            <img
              src="@/assets/img/avadabarbers-trimcut-before.png"
              alt="trimcut"
            />
          </figure>
          <h3>Trim & Cut</h3>
          <p class="lh-lg mt-4 fs-5">
            Avada Barbers are experts in the lickety split trim and hair cut.
            Quick but careful and ridiculously good looking.
          </p>
        </div>
        <div class="col-4 p-5">
          <figure>
            <img src="@/assets/img/avadabarbers-washndry.png" alt="washndry" />
          </figure>
          <h3>Wash & Dry</h3>
          <p class="lh-lg mt-4 fs-5">
            Take a seat in our fine leather chairs, lean back and let us lather
            you a fresh head in a luxurious fashion.
          </p>
        </div>
        <div class="col-4 p-5">
          <figure>
            <img
              src="@/assets/img/avadabarbers-beardtrim.png"
              alt="beardtrim"
            />
          </figure>
          <h3>Beard Tidy</h3>
          <p class="lh-lg mt-4 fs-5">
            Tame the tangles and untidy facial hairs like a gentleman with our
            Beard Tidy services from Avada Barbers.
          </p>
        </div>
        <!-- BOTTONE 'SCOPRI I SERVIZI' -->
        <div class="col-12">
          <div class="button-services text-uppercase py-3 px-5 my-5">
            <ButtonLg>
              Read About Our Services
            </ButtonLg>
          </div>
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
          style="fill:#121314;padding:0;"
        >
          <path d="M0 100 L50 2 L100 100 Z" />
        </svg>
      </div>
    </div>
  </section>
</template>

<script>
import ButtonLg from "@/components/ButtonLg.vue";
export default {
  name: "SectionServices",
   components: {
    ButtonLg,
  },
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";
// BACKGROUND
#services {
  padding: 50px 0 170px 0;
}

// IMMAGINI
figure img {
  height: 150px;
}

//POSIZIONAMENTO SVG
svg {
  bottom: 0;
  left: 0;
}
</style>

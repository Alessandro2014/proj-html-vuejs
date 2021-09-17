<template>
  <footer id="top-footer">
    <div class="container">
      <div class="row text-center">
        <!-- COLONNE SHOP -->
        <div
          class="col-5 d-flex flex-column justify-content-end py-5 d-grid gap-4"
        >
          <figure class="m-0">
            <img
              src="@/assets/img/avadabarbers_footer_shop_image-400x312.png"
              alt="avadabarbers-logo-200x70"
            />
          </figure>
          <div>
            <ButtonLg>
              shop our range now
            </ButtonLg>
          </div>
        </div>
        <!-- COLONNA CONTATTI -->
        <div
          class="col-2 d-flex flex-column justify-content-end py-5 d-grid gap-4"
        >
          <figure>
            <img :src="logo" alt="avadabarbers-logo-200x70" />
          </figure>
          <p class="lh-lg">
            Avada Barbers <br />
            123 New York Street <br />
            New York City <br />
            info@yourwebsite.com <br />
            +1 (555) 555-1212
          </p>
          <h4>FOLLOW US</h4>
          <div class="d-flex justify-content-around text-white fs-5 py-3">
            <i class="fab fa-facebook-f"></i>
            <i class="fab fa-twitter"></i>
            <i class="fab fa-youtube"></i>
            <i class="fab fa-instagram"></i>
          </div>
        </div>
        <!-- COLONNA APPUNTAMENTI -->
        <div
          class="col-5 d-flex flex-column justify-content-end py-5 d-grid gap-4"
        >
          <figure class="m-0">
            <img
              src="@/assets/img/avadabarbers_footer_appointment_image-400x312.png"
              alt="avadabarbers-logo-200x70"
            />
          </figure>
          <div>
            <ButtonLg>
              book your appointment
            </ButtonLg>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import ButtonLg from "@/components/ButtonLg.vue";
export default {
  name: "Footer",
  props: ["logo"],
  components: {
    ButtonLg,
  },
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";
#top-footer {
  background-color: black;
}

// IMMAGINI
img {
  height: auto;
  max-width: 100%;
  margin: 0;
}
</style>

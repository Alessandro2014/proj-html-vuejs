<template>
  <footer id="top-footer">
    <div class="container">
      <div class="row text-center">
        <!-- COLONNE SHOP -->
        <div
          class="col-4 d-flex flex-column justify-content-center py-5 d-grid gap-4"
        >
          <figure>
            <img
              src="@/assets/img/avadabarbers_footer_shop_image-400x312.png"
              alt="avadabarbers-logo-200x70"
              class="img-fluid"
            />
          </figure>
          <div>
            <div class="button-blog text-uppercase py-3 px-5">
              <a href="#">shop our range now</a>
            </div>
          </div>
        </div>
        <!-- COLONNA CONTATTI -->
        <div
          class="col-4 d-flex flex-column justify-content-center py-5 d-grid gap-4"
        >
          <figure>
            <img
              src="@/assets/img/avadabarbers-logo-200x70.png"
              alt="avadabarbers-logo-200x70"
              class="img-fluid"
            />
          </figure>
          <p class="lh-lg">
            Avada Barbers <br />
            123 New York Street <br />
            New York City <br />
            info@yourwebsite.com <br />
            +1 (555) 555-1212
          </p>
          <h4>FOLLOW US</h4>
          <div class="d-flex justify-content-evenly text-white fs-5 py-3 px-5">
            <i class="fab fa-facebook-f"></i>
            <i class="fab fa-twitter"></i>
            <i class="fab fa-youtube"></i>
            <i class="fab fa-instagram"></i>
          </div>
        </div>
        <!-- COLONNA APPUNTAMENTI -->
        <div
          class="col-4 d-flex flex-column justify-content-center py-5 d-grid gap-4"
        >
          <figure>
            <img
              src="@/assets/img/avadabarbers_hero_focalmirror-200x275.png"
              alt="avadabarbers-logo-200x70"
              class="img-fluid"
            />
          </figure>
          <div>
            <div class="button-blog text-uppercase py-3 px-5">
              <a href="#">book your appointment</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";
#top-footer {
  background-color: black;
}

h4 {
  color: $important;
  font-family: $font-general;
  font-size: 1.1rem;
}

p {
  font-family: $font-general;
  color: $regular;
  font-weight: 300;
}

img {
  height: auto;
  max-width: 150px;
  margin-bottom: 20px;
}

.button-blog {
  border: 2px solid $important;
  display: inline-block;
  a {
    color: $important;
    font-family: $font-general;
    text-decoration: none;
    font-weight: 600;
  }
}
</style>

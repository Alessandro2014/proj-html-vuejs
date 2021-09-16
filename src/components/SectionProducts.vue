<template>
  <!-- SEZIONE  products-->
  <section id="products">
    <div class="container">
      <!-- COLONNA TITOLO -->
      <div class="row text-center">
        <div class="col-12 py-1">
          <h4>WE HAVE YOU COVERED</h4>
        </div>
        <div class="col-12 py-1">
          <h2>Avada Grooming Products</h2>
        </div>
        <!-- COLONNE VETRINA PRODOTTI -->
        <div class="col-3 py-5">
          <figure>
            <img src="@/assets/img/brush_dark-400x400.png" alt="brush_dark" />
          </figure>
          <figcaption>Trim & Cut</figcaption>
          <p>
            $ 15.00
          </p>
        </div>
        <div class="col-3 py-5">
          <figure>
            <img src="@/assets/img/scissors-400x400.png" alt="scissors" />
          </figure>
          <figcaption>Wash & Dry</figcaption>
          <p>
            $ 85.00
          </p>
        </div>
        <div class="col-3 py-5">
          <figure>
            <img
              src="@/assets/img/hot_oil_dark-400x400.png"
              alt="hot_oil_dark"
            />
          </figure>
          <figcaption>Beard Tidy</figcaption>
          <p>
            $ 15.00
          </p>
        </div>
        <div class="col-3 py-5">
          <figure>
            <img
              src="@/assets/img/straight_razor_dark-400x400.png"
              alt="straight_razor_dark"
            />
          </figure>
          <figcaption>Beard Tidy</figcaption>
          <p>
            $ 30.00
          </p>
        </div>
        <!-- BOTTONE 'SHOP PRODOTTI' -->
        <div class="col-12">
          <div class="button-products text-uppercase py-3 px-5 my-5">
            <a href="#">Shop Our Product Range</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionProducts",
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";
// BACKGROUND
#products {
  background-image: url("../assets/img/avadabarbers-reviewsbackground.jpg");
  background-size: cover;
  background-position: top;
  background-repeat: no-repeat;
  padding: 70px 0;
}
// TESTO
h2 {
  font-size: 4.5rem;
  color: $title;
  font-family: $font-avada;
}

h4 {
  color: $important;
  font-family: $font-general;
  font-size: 1.1rem;
}

figcaption {
  color: $important;
  font-family: $font-avada;
  font-size: 2rem;
}

p {
  font-size: 1.2rem;
  font-family: $font-general;
  color: $important;
}

.button-products {
  border: 2px solid $important;
  display: inline-block;
  a {
    color: $important;
    font-family: $font-general;
    text-decoration: none;
    font-weight: 600;
  }
}

// IMMAGINI
figure img {
  height: 300px;
  width: auto;
}
</style>

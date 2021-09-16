<template>
  <section>
    <!-- SEZIONE  PRODOTTI-->
    <section id="products">
      <div class="container-fluid">
        <!-- COLONNA TITOLO -->
        <div class="row text-center px-3">
          <div class="col-12 py-1">
            <h4>WE HAVE YOU COVERED</h4>
          </div>
          <div class="col-12 py-1">
            <h2>Avada Grooming Products</h2>
          </div>
          <!-- COLONNE VETRINA PRODOTTI -->
          <div class="col-3 py-5">
            <img
              src="@/assets/img/brush_dark-400x400.png"
              alt="brush_dark"
              class="img-fluid"
            />
            <figcaption>Trim & Cut</figcaption>
            <p>
              $ 15.00
            </p>
          </div>
          <div class="col-3 py-5">
            <img
              src="@/assets/img/scissors-400x400.png"
              alt="scissors"
              class="img-fluid"
            />
            <figcaption>Wash & Dry</figcaption>
            <p>
              $ 85.00
            </p>
          </div>
          <div class="col-3 py-5">
            <img
              src="@/assets/img/hot_oil_dark-400x400.png"
              alt="hot_oil_dark"
              class="img-fluid"
            />
            <figcaption>Beard Tidy</figcaption>
            <p>
              $ 15.00
            </p>
          </div>
          <div class="col-3 py-5">
            <img
              src="@/assets/img/straight_razor_dark-400x400.png"
              class="img-fluid"
              alt="straight_razor_dark"
            />
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
    <!-- SEZIONE PRODOTTO DEL MESE-->
    <section>
      <div id="product-window" class="container">
        <div class="row">
          <div class="col-5 text-center img-product">
            <img
              src="@/assets/img/shaving_butter-400x400.png"
              alt="shaving_butter"
              class="img-fluid"
            />
          </div>
          <div
            class="
                product-description
                col-7
                d-flex
                align-items-start
                flex-column
                justify-content-center
                d-grid
                gap-2
                "
          >
            <h4>THIS MONTHS FEATURED PRODUCT</h4>
            <h2 class="pb-2">Shaving Butter</h2>
            <p class="lh-lg mt-4 fs-5">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Pellentesque laoreet enim est, vel molestie dolor ultrices ut.
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
            </p>
            <div class="button-now text-uppercase py-3 px-5">
              <a href="#">BUY NOW</a>
            </div>
          </div>
        </div>
      </div>
    </section>
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

#products p {
  font-size: 1.2rem;
  font-family: $font-general;
  color: $important;
}

#product-window p {
  font-family: $font-general;
  color: $regular;
  font-weight: 300;
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

//  SEZIONE PRODOTTO DEL MESE
#product-window {
  background-color: black;
  margin-top: -50px;  
  border-top: 4px solid $important;
  max-width: 1300px;
  max-height: 500px;

}

.img-product {
  background-image: url("../assets/img/avadabarbers-cta-background.jpg");
  background-size: cover;
  background-position: left;
  background-repeat: no-repeat;
  padding: 70px 0;
  max-height: 500px;
}

.product-description {
    padding: 70px;
}

.button-now {
  border: 2px solid $important;
  a {
    color: $important;
    font-family: $font-general;
    text-decoration: none;
    font-weight: 400;
  }
}
</style>

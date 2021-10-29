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
          <!-- COLONNE VETRINA PRODOTTI STAMPA CON DATI DINAMICI-->
          <div
            v-for="(product, index) in products"
            :key="index"
            class="col-3 py-5"
          >
            <img
              :src="getUrlImg(product.img)"
              :alt="product.name"
              class="img-fluid"
            />
            <figcaption>{{ product.name }}</figcaption>
            <p>
              {{ product.price }}
            </p>
          </div>
          <!-- BOTTONE 'SHOP PRODOTTI' -->
          <div class="col-12">
            <ButtonLg>
              Shop Our Product Range
            </ButtonLg>
          </div>
        </div>
      </div>
    </section>
    <!-- SEZIONE PRODOTTO DEL MESE-->
    <section>
      <div id="product-window" class="container mb-5">
        <div class="row">
          <div class="col-5 text-center img-product">
            <img
              src="@/assets/img/shaving_butter-400x400.png"
              alt="shaving_butter"
            />
          </div>
          <div
            class="
                description-product
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
            <div class="text-uppercase">
              <ButtonLg>
                buy now
              </ButtonLg>
            </div>
          </div>
        </div>
      </div>
    </section>
  </section>
</template>

<script>
import ButtonLg from "@/components/ButtonLg.vue";
export default {
  name: "SectionProducts",
  data() {
    return {
      // DETTAGLIO PRODOTTI
      products: [
        {
          img: "brush_dark-400x400.png",
          name: "Trim & Cut",
          price: "$ 15.00",
          current: true,
        },
        {
          img: "scissors-400x400.png",
          name: "Wash & Dry",
          price: "$ 85.00",
          current: true,
        },
        {
          img: "hot_oil_dark-400x400.png",
          name: "Beard Tidy",
          price: "$ 15.00",
          current: true,
        },
        {
          img: "straight_razor_dark-400x400.png",
          name: "Beard Tidy",
          price: "$ 30.00",
          current: true,
        },
      ],
    };
  },
  components: {
    ButtonLg,
  },
  methods: {
    getUrlImg(fileName) {
      return require("@/assets/img/" + fileName);
    },
  },
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";

// BACKGROUND
#products {
  background-image: url("../assets/img/avadabarbers-reviewsbackground.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  padding: 70px 0 120px;
}

#products p {
  color: $important;
}

//  SEZIONE PRODOTTO DEL MESE
#product-window {
  background-color: black;
  margin-top: -50px;
  border-top: 4px solid $important;
  max-width: 1200px;
  height: 510px;
}

.description-product {
  padding: 60px;
}

.img-product {
  background-image: url("../assets/img/avadabarbers-cta-background.jpg");
  background-size: cover;
  background-position: left;
  background-repeat: no-repeat;
  height: 505px;
  img {
    height: 500px;
  }
}
</style>

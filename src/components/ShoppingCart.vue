<template>
  <div>
    <!-- BOTTONI LATERALI -->
    <div
      class="button-info rounded-3 shadow-lg cursor position-fixed d-flex flex-column justify-content-around text-center"
    >
      <!-- DEMO + CARRELLO -->
      <i class="fas fa-file-video fs-3"></i>
      <p class="m-0">{{ info }}</p>
    </div>
    <div
      class="button-cart rounded-3 shadow-lg cursor position-fixed d-flex flex-column justify-content-around text-center"
    >
      <!--CARRELLO -->

      <span class="price fs-3"><sup>$</sup>{{ value }}</span>
      <p class="m-0">{{ cart }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "ShoppingCart",
  props: ["info", "cart", "value"],
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";

// POSIZIONAMENTO E LAYOUT BOTTONI
.button-info,
.button-cart {
  background-color: $popular;
  right: 15px;
  padding: 8px 5px;
  width: 65px;
  height: 65px;
  font-size: 0.8rem;
  z-index: 2;
}

.button-info {
  top: 140px;
}

.button-cart {
  top: 220px;
}

.price {
  color: $price;
  font-weight: 600;
}
</style>

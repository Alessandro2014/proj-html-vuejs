<template>
  <div>
    <div
      class="button-info  cursor position-fixed d-flex flex-column justify-content-between text-center"
    >
      <i class="fas fa-file-video fs-3"></i>
      {{ info }}
    </div>
    <div
      class="button-cart  cursor position-fixed d-flex flex-column justify-content-between text-center"
    >
      <span class="price fs-3"><sup>$</sup>{{ value }}</span>
      {{ cart }}
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

.button-info,
.button-cart {
  background-color: $popular;
  right: 10px;
  padding: 8px 6px;
  width: 65px;
  height: 65px;
  border-radius: 5px;
  font-size: 0.8rem;
}

.button-info {
  top: 140px;
}

.button-cart {
  top: 220px;
}

.price {
  color: $price;
  font-weight: 800;
}
</style>

<template>
    <div class="card col-3 py-5">
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
</template>

<script>
export default {
name: "ProductCard",
props: ["product"],
  methods: {
    getUrlImg (fileName) {
      return require("@/assets/img/" + fileName);
    }
  },
}
</script>

<style scoped lang="scss">
@import "../scss/style.scss";
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
</style>
<template>
  <!-- SEZIONE  BLOG-->
  <section id="blog" class="position-relative">
    <div class="container">
      <!-- COLONNA TITOLO -->
      <div class="row text-center">
        <div class="col-12">
          <h4>TALES FROM THE BARBER SHOP</h4>
        </div>
        <div class="col-12 pb-5">
          <h2>Recent Blog Posts</h2>
        </div>
        <!-- COLONNE DESCRIZIONE BLOG -->
        <div class="col-4">
          <img
            src="@/assets/img/avadabarbers-second-blog-700x441.jpg"
            alt="trimcut"
          />
          <h3>Avada Barbers Now Open</h3>
          <p class="lh-lg mt-4 fs-5">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus
            ut dapibus magna. Praesent semper,
          </p>
        </div>
        <div class="col-4">
          <img
            src="@/assets/img/avadabarbers-choosing-blog-700x441.jpg"
            alt="washndry"
          />
          <h3>Choosing The Right Barber</h3>
          <p class="lh-lg mt-4 fs-5">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus
            ut dapibus magna. Praesent semper,
          </p>
        </div>
        <div class="col-4">
          <img
            src="@/assets/img/avadabarbers-ourservice-blog-700x441.jpg"
            alt="beardtrim"
          />
          <h3>Quick Service Guide</h3>
          <p class="lh-lg mt-4 fs-5">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus
            ut dapibus magna. Praesent semper,
          </p>
        </div>
        <!-- BOTTONE 'SCOPRI I BLOG' -->
        <div class="col-12">
          <ButtonLg class="button">
            Read More From Our Blog
          </ButtonLg>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import ButtonLg from "@/components/ButtonLg.vue";
export default {
  name: "SectionBlog",
  components: {
    ButtonLg,
  },
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";
// BACKGROUND
#blog {
  background-color: #eae8e6;
  padding: 170px 0 70px;
}

// IMMAGINI
img {
  height: auto;
  max-width: 400px;
  margin-bottom: 20px;
}

//POSIZIONAMENTO SVG
svg {
  bottom: 0;
  left: 0;
  background-color: #eae8e6;
}
</style>

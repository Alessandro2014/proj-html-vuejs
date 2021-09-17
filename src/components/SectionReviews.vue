<template>
  <!-- SEZIONE  REVIEWS-->
  <section id="reviews" class="position-relative">
    <div class="container">
      <!-- COLONNA TITOLO -->
      <div class="row text-center">
        <div class="col-12 mt-5">
          <h4>WHAT PEOPLE SAY</h4>
        </div>
        <div class="col-12 py-3">
          <h2>Reviews</h2>
        </div>
        <!-- COLONNE DESCRIZIONE SERVIZI -->
        <div class="col-4 p-5">
          <p class="lh-lg mt-4 fs-5">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi
            mollis eleifend ante ut sagittis. Sed sodales, urna et imperdiet
            placerat, ex nisi aliquam orci, ac varius odio libero et arcu.
          </p>
            <img
              src="@/assets/img/avadabarbers-trimcut-gallery6-200x200.jpg"
              alt="trimcut" class="rounded-circle "
            />
          <h3>John Doe</h3>
        </div>
        <div class="col-4 p-5">
          <p class="lh-lg mt-4 fs-5">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi
            mollis eleifend ante ut sagittis. Sed sodales, urna et imperdiet
            placerat, ex nisi aliquam orci, ac varius odio libero et arcu.
          </p>
            <img
              src="@/assets/img/avadabarbers-trimcut-gallery7-200x201.jpg"
              alt="washndry" class="rounded-circle "
            />
          <h3>Pete Jones</h3>
        </div>
        <div class="col-4 p-5">
          <p class="lh-lg mt-4 fs-5">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi
            mollis eleifend ante ut sagittis. Sed sodales, urna et imperdiet
            placerat, ex nisi aliquam orci, ac varius odio libero et arcu.
          </p>
            <img
              src="@/assets/img/avadabarbers-trimcut-gallery3-200x201.jpg"
              alt="beardtrim" class="rounded-circle "
            />
          <h3>Mark Wilson</h3>
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
          style="fill:#fcfcfc;padding:0;"
        >
          <path d="M0 100 L50 2 L100 100 Z" />
        </svg>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionReviews",
};
</script>

<style scoped lang="scss">
@import "../scss/style.scss";
// BACKGROUND
#reviews {
  padding: 50px 0 170px 0;
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

h3 {
  color: $important;
  font-family: $font-avada;
  font-size: 1.5rem;
  padding: 3rem 0;
  font-style: italic;
}

p {
  font-family: $font-general;
  color: $regular;
  font-weight: 300;
}

// IMMAGINI
img {
  max-width: 110px;
  height: auto;
}

//POSIZIONAMENTO SVG
svg {
   bottom: 0;
  left: 0;
  transform: rotate(180deg);
  background-color: #eae8e6;
}
</style>

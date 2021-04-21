<template>
  <div class="home">
    <section class="hero is-light shadow">
      <div class="hero-body">
        <div class="container">
          <div
            id="carouselExampleIndicators"
            class="carousel slide carousel-fade"
            data-bs-ride="carousel"
          >
            <div class="carousel-indicators">
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="0"
                class="active"
                aria-current="true"
                aria-label="Slide 1"
              ></button>
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="1"
                aria-label="Slide 2"
              ></button>
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="2"
                aria-label="Slide 3"
              ></button>
            </div>
            <div class="carousel-inner">
              <div class="carousel-item active">
                <img src="../assets/img/banner/banner1.jpg" alt="..." />
              </div>
              <div class="carousel-item">
                <img src="../assets/img/banner/banner2.jpg" alt="..." />
              </div>
              <!-- <div class="carousel-item">
                <img src="..." class="d-block w-100" alt="..." />
              </div> -->
            </div>
            <button
              class="carousel-control-prev"
              type="button"
              data-bs-target="#carouselExampleIndicators"
              data-bs-slide="prev"
            >
              <span
                class="carousel-control-prev-icon"
                aria-hidden="true"
              ></span>
              <span class="visually-hidden">Previous</span>
            </button>
            <button
              class="carousel-control-next"
              type="button"
              data-bs-target="#carouselExampleIndicators"
              data-bs-slide="next"
            >
              <span
                class="carousel-control-next-icon"
                aria-hidden="true"
              ></span>
              <span class="visually-hidden">Next</span>
            </button>
          </div>
        </div>
      </div>
    </section>
  
    <section class="container mt-5 p-5 shadow">
      <iframe src="//vt.plushglobalmedia.com/tour/TT17LMCOIA" width="100%" height="450" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true" allowvr="yes" allow="vr; xr; accelerometer; gyroscope;"><p>Your browser does not support iframes.</p></iframe>
    </section>

    <section class="container mt-4 p-6">
      <Access />
    </section>

    <section class="hero border-0 mt-6 p-5 is-trasnparent shadow-lg">
      <div class="columns">
        <div class="column">
          <h1>Redes Sociales</h1>
          <div></div>

          <hr />
          <h2>Encuentranos en:</h2>
          <p>
            Pedro Ávila y Sebastián de Benalcazar
            <br />
            La Armenia – 170803
            <br />
            (593) 2 393 1060
            <br />
            info@uegonzaga.edu.ec
          </p>
        </div>
        <div class="column">
          <figure class="image">
            <img src="../assets/img/posts/Sermasservirmejor.png" alt="" />
          </figure>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
import Access from "../components/Access.vue";

export default {
  name: "home",
  components: {
    Access,
  },
};
</script>
<style lang="scss" scoped>
.carousel-control-prev-icon .carousel-control-next-icon {
  height: 5rem !important;
}
</style>

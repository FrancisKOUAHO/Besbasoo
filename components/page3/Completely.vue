<template>
  <div class="slider-completely">
    <h1>Les utilisateurs ont également consulté...</h1>

      <VueSlickCarousel
        :arrows="true"
        v-bind="settings"
        class="vue-slick-carousel"
      >
        <div class="box" style="margin: 4rem;" v-for="slider in 5">
          <h3>Sculpture Femme Africaine Watusi nue  - ANZENGRUBER KERAMIK</h3>
          <img src="~/assets/images/image-14.png" alt="" class="img-shadow-ribbon">
          <p>Avant : <span class="price-barre-box">79,99€</span> (-20%)</p>
          <div class="box-price">
            <p class="box-tilte">55,99€</p>
            <p class="box-delivery">
              <svg id="Capa_1" enable-background="new 0 0 512 512" height="30" viewBox="0 0 512 512" width="30" xmlns="http://www.w3.org/2000/svg"><g><path d="m407 16c-57.891 0-105 47.109-105 105s47.109 105 105 105 105-47.109 105-105-47.109-105-105-105zm45 120h-30v30h-30v-30h-30v-30h30v-30h30v30h30z"/><path d="m137 376c8.3 0 292.767 0 281.602 0l33.252-128.247c-10.422 3.702-21.396 6-32.807 7.029l-.315 1.218h-70.437l1.117-13.391c-10.366-4.933-19.834-11.239-28.546-18.532l-2.661 31.923h-62.41l-5.001-60h44.059c-6.172-9.201-10.779-19.396-14.561-30h-141.261l-20.004-90h-119.027v30h94.974l53.32 240h-11.294c-24.814 0-45 20.186-45 45s20.186 45 45 45h17.763c-1.681 4.715-2.763 9.716-2.763 15 0 24.814 20.186 45 45 45s45-20.186 45-45c0-5.284-1.082-10.285-2.763-15h65.526c-1.681 4.715-2.763 9.716-2.763 15 0 24.814 20.186 45 45 45s45-20.186 45-45c0-5.284-1.082-10.285-2.763-15h32.763v-30h-285c-8.276 0-15-6.724-15-15s6.724-15 15-15zm208.795-90h65.158l-15.555 60h-54.604zm-30.09 0-5.001 60h-47.41l-5.001-60zm-82.5 60h-54.168l-13.336-60h62.503zm-87.507-150h75.007l5.001 60h-66.671zm66.302 255c0 8.276-6.724 15-15 15s-15-6.724-15-15 6.724-15 15-15 15 6.724 15 15zm150 0c0 8.276-6.724 15-15 15s-15-6.724-15-15 6.724-15 15-15 15 6.724 15 15z"/></g></svg>
            </p>
          </div>
          <div class="cross-shadow-ribbon">PROMO</div>
        </div>
      </VueSlickCarousel>
    </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
  name: "Completely",
  components: {VueSlickCarousel},
  data() {
    return {
      settings: {
        "infinite": true,
        "initialSlide": 2,
        "speed": 500,
        "slidesToShow": 3,
        "slidesToScroll": 1,
        "swipeToSlide": true
      }
    }
  },
}
</script>

<style lang="scss">
.slider-completely {
  margin: 1rem auto;
  padding: 2rem;
  font-family: Rambla, serif;

  h1 {
    font-size: 30px;
    font-weight: bold;
  }

  .vue-slick-carousel {
    width: 1300px;
    height: 280px;
    margin-left: auto;
    margin-right: auto;
    margin-top: 2rem;

    .box-price{
      display: flex;
      justify-content: space-between;

    }

    .box-delivery{
      color: #ff9a24;
    }
    .box-tilte{
      color: #ff9a24;
      font-weight: bold;
      font-size: 25px;
    }

    .img-shadow-ribbon{
      margin-left: auto;
      margin-right: auto;
    }

    .price-barre-box {
      font-family: Rambla, serif;
      text-decoration: line-through;
      font-size: 13px;
    }

    .slick-arrow {
      width: 2rem;
      color: #e40000 !important;
      background: #e40000 !important;
      margin-left: -1rem;
      height: 3rem;
    }

    .slick-next {
      width: 2rem;
      color: #e40000 !important;
      background: #e40000 !important;
      margin-right: -1rem;
      height: 3rem;
    }

    .box {
      width: 80% !important;
      padding: 1rem;
      border: 1px solid #CCC;
      background: #FFF;
      height: 290px;
      position: relative;
      border-radius: 3px;
    }

    .cross-shadow-ribbon {
      position: absolute;
      background: #E40000;
      top: 8em;
      left: -2.9em;
      padding: 8px 15px;
      text-align: center;
      color: #FFF;
      transform: rotate(-90deg)
    }

    .cross-shadow-ribbon:before {
      content: "";
      position: absolute;
      left: -20px;
      right: 0;
      top: 0;
      bottom: 0;
      width: 0;
      height: 0;
      border-bottom: 20px solid #ab0202;
      border-left: 20px solid transparent;
    }


  }


}

</style>

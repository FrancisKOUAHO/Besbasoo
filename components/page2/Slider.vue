<template>
  <div
    class="w-full  bg-gradient-to-r from-gray-900 via-gray-900 to-gray-900 slider-background"
    style=" height: 494px;"
  >
    <div class="mySlides w-full text-center">
      <div class=" w-full  text-center  py-5  ">
        <p class="text-5xl font-bold py-10 text-white">Alimentaires</p>
        <p class=" leading-loose text-white">
          Profitez des réductions sur la gamme alimentaire pour satisfaire les
          papilles de vos proches
          <br />
          Jusqu’à -70 %

          <br />
          Jusqu’au 31 mai 2021
        </p>
        <br />
        <center>
          <div class="w-80 h-16">
            <div
              class="relative bg-yellow-500 rounded"
              style="width: 352px; height: 64px;"
            >
              <p
                class="absolute text-xl leading-relaxed text-center text-white"
                style="left: 20px; top: 19px;"
              >
                Plus que
              </p>

              <p
                class="w-7 h-7 bg-white  absolute text-2xl font-bold leading-relaxedtext-center text-gray-900"
                style="left: 118px; top: 14px;"
              >
                05
              </p>
              <p
                class="w-7  h-7 bg-white absolute text-2xl font-bold leading-relaxed text-center text-gray-900"
                style="left: 175px; top: 14px;"
              >
                21
              </p>
              <p
                class="w-7  h-7 bg-white absolute text-2xl font-bold leading-relaxed text-center text-gray-900"
                style="left: 236px; top: 14px;"
              >
                29
              </p>
              <p
                class="w-7  h-7 bg-white absolute text-2xl font-bold leading-relaxed text-center text-gray-900"
                style="left: 294px; top: 14px;"
              >
                15
              </p>
              <p
                class="absolute text-xs leading-relaxed text-center text-white"
                style="left: 120px; top: 38px;"
              >
                Jours
              </p>
              <p
                class="absolute text-xs leading-relaxed text-center text-white"
                style="left: 175px; top: 38px;"
              >
                Heures
              </p>
              <p
                class="absolute text-xs leading-relaxed text-center text-white"
                style="left: 231px; top: 38px;"
              >
                Minutes
              </p>
              <p
                class="absolute text-xs leading-relaxed text-center text-white"
                style="left: 288px; top: 38px;"
              >
                Secondes
              </p>
            </div>
          </div>
        </center>
      </div>
    </div>
    <!--
    <div class="mySlides w-full">
      <q>I have not failed. I've just found 10,000 ways that won't work.</q>
    </div> -->

    <div class="mySlides w-full">
      <!-- <q>I have not failed. I've just found 10,000 ways that won't work.</q> -->
    </div>

    <a class="prev left-0" @click="showSlides(-1)">❮</a>
    <a class="next" @click="showSlides(1)">❯</a>
  </div>
</template>
<script>
export default {
  data() {
    return {
      slideIndex: 1
    };
  },
  mounted() {
    this.showSlides(1);
  },
  methods: {
    showSlides(n) {
      var i;
      var slides = document.getElementsByClassName("mySlides");

      if (n > slides.length) {
        this.slideIndex = 1;
      }
      if (n < 1) {
        this.slideIndex = slides.length;
      }
      for (i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";
      }

      slides[this.slideIndex - 1].style.display = "block";
    }
  }
};
</script>

<style scoped>

.slider-background{
  background: url("~/assets/images/Fond.png");
}

.prev,
.next {
  cursor: pointer;
  position: absolute;
  background-color: #787878;
  top: 50%;
  width: auto;
  padding: 16px;
  color: #fff;
  font-size: 25px;
  border-radius: 0 3px 3px 0;
  user-select: none;
}

.next {
  position: absolute;
  right: 0;
  border-radius: 3px 0 0 3px;
}

.prev:hover,
.next:hover {
  background-color: rgba(0, 0, 0, 0.8);
  color: white;
}
</style>

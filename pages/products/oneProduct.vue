<template>
  <section>
    <div class="section-oneProduct">
      <div class="picture-secondes">
        <div class="box-picture"><img src="~/assets/images/image-14.png" alt=""></div>
        <div class="box-picture"><img src="~/assets/images/image-14.png" alt=""></div>
        <div class="box-picture"><img src="~/assets/images/image-14.png" alt=""></div>
        <div class="box-picture"><img src="~/assets/images/image-14.png" alt=""></div>
        <div class="box-picture"><img src="~/assets/images/image-14.png" alt=""></div>
      </div>

      <div class="picture-principal">
        <img src="~/assets/images/image-14.png" alt="">
        <div class="cercle">
          <button class="toggle-favorite" @click="toggle">
            <FavoriteIcon
              class="toggle-favorite__icon heart"
              :class="iconClasses"
              @animationend.native="onIconAnimationEnds"
              width="30"
            />
            <transition name="favorite-particles-transition">
              <div v-if="animating" class="toggle-favorite__particles"></div>
            </transition>
          </button>
        </div>
      </div>

      <div class="description-principal">
        <h1>Sculpture Femme Africaine Watusi nue - ANZENGRUBER KERAMIK</h1>

        <div class="group-stars">
        <span v-for="star in 4">
           <svg class="mx-1 w-4 h-4 fill-current text-yellow-500" xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 20 20">
          <path
            d="M10 15l-5.878 3.09 1.123-6.545L.489 6.91l6.572-.955L10 0l2.939 5.955 6.572.955-4.756 4.635 1.123 6.545z"/>
        </svg>
        </span>
          <svg class="mx-1 w-4 h-4 fill-current text-gray-400" xmlns="http://www.w3.org/2000/svg"
               viewBox="0 0 20 20">
            <path
              d="M10 15l-5.878 3.09 1.123-6.545L.489 6.91l6.572-.955L10 0l2.939 5.955 6.572.955-4.756 4.635 1.123 6.545z"/>
          </svg>
          <div class="avis-product">46 avis</div>
          <div class="share">
            <svg height="20" viewBox="-21 0 512 512" width="20" xmlns="http://www.w3.org/2000/svg">
              <path
                d="m453.332031 85.332031c0 38.292969-31.039062 69.335938-69.332031 69.335938s-69.332031-31.042969-69.332031-69.335938c0-38.289062 31.039062-69.332031 69.332031-69.332031s69.332031 31.042969 69.332031 69.332031zm0 0"/>
              <path
                d="m384 170.667969c-47.0625 0-85.332031-38.273438-85.332031-85.335938 0-47.058593 38.269531-85.332031 85.332031-85.332031s85.332031 38.273438 85.332031 85.332031c0 47.0625-38.269531 85.335938-85.332031 85.335938zm0-138.667969c-29.417969 0-53.332031 23.9375-53.332031 53.332031 0 29.398438 23.914062 53.335938 53.332031 53.335938s53.332031-23.9375 53.332031-53.335938c0-29.394531-23.914062-53.332031-53.332031-53.332031zm0 0"/>
              <path
                d="m453.332031 426.667969c0 38.289062-31.039062 69.332031-69.332031 69.332031s-69.332031-31.042969-69.332031-69.332031c0-38.292969 31.039062-69.335938 69.332031-69.335938s69.332031 31.042969 69.332031 69.335938zm0 0"/>
              <path
                d="m384 512c-47.0625 0-85.332031-38.273438-85.332031-85.332031 0-47.0625 38.269531-85.335938 85.332031-85.335938s85.332031 38.273438 85.332031 85.335938c0 47.058593-38.269531 85.332031-85.332031 85.332031zm0-138.667969c-29.417969 0-53.332031 23.9375-53.332031 53.335938 0 29.394531 23.914062 53.332031 53.332031 53.332031s53.332031-23.9375 53.332031-53.332031c0-29.398438-23.914062-53.335938-53.332031-53.335938zm0 0"/>
              <path
                d="m154.667969 256c0 38.292969-31.042969 69.332031-69.335938 69.332031-38.289062 0-69.332031-31.039062-69.332031-69.332031s31.042969-69.332031 69.332031-69.332031c38.292969 0 69.335938 31.039062 69.335938 69.332031zm0 0"/>
              <path
                d="m85.332031 341.332031c-47.058593 0-85.332031-38.269531-85.332031-85.332031s38.273438-85.332031 85.332031-85.332031c47.0625 0 85.335938 38.269531 85.335938 85.332031s-38.273438 85.332031-85.335938 85.332031zm0-138.664062c-29.417969 0-53.332031 23.933593-53.332031 53.332031s23.914062 53.332031 53.332031 53.332031c29.421875 0 53.335938-23.933593 53.335938-53.332031s-23.914063-53.332031-53.335938-53.332031zm0 0"/>
              <path
                d="m135.703125 245.761719c-7.425781 0-14.636719-3.863281-18.5625-10.773438-5.824219-10.21875-2.238281-23.253906 7.980469-29.101562l197.949218-112.851563c10.21875-5.867187 23.253907-2.28125 29.101563 7.976563 5.824219 10.21875 2.238281 23.253906-7.980469 29.101562l-197.953125 112.851563c-3.328125 1.898437-6.953125 2.796875-10.535156 2.796875zm0 0"/>
              <path
                d="m333.632812 421.761719c-3.585937 0-7.210937-.898438-10.539062-2.796875l-197.953125-112.851563c-10.21875-5.824219-13.800781-18.859375-7.976563-29.101562 5.800782-10.238281 18.855469-13.84375 29.097657-7.976563l197.953125 112.851563c10.21875 5.824219 13.800781 18.859375 7.976562 29.101562-3.945312 6.910157-11.15625 10.773438-18.558594 10.773438zm0 0"/>
            </svg>
          </div>
        </div>
        <p class="stock">En stock (encore 20 disponibles)</p>
        <p class="free-delivery"><strong>Livraison gratuite</strong>en France métropolitaine et DOM</p>
        <p class="free-delivery"><strong>Délais : </strong>3-4 jours ouvrés</p>
        <p class="free-delivery">Estimation :<strong> jeudi 17 juin</strong></p>

        <div class="select-adress">
          <svg id="Layer_1" enable-background="new 0 0 512 512" height="14" viewBox="0 0 512 512" width="14"
               xmlns="http://www.w3.org/2000/svg">
            <g>
              <path
                d="m407.579 87.677c-31.073-53.624-86.265-86.385-147.64-87.637-2.62-.054-5.257-.054-7.878 0-61.374 1.252-116.566 34.013-147.64 87.637-31.762 54.812-32.631 120.652-2.325 176.123l126.963 232.387c.057.103.114.206.173.308 5.586 9.709 15.593 15.505 26.77 15.505 11.176 0 21.183-5.797 26.768-15.505.059-.102.116-.205.173-.308l126.963-232.387c30.304-55.471 29.435-121.311-2.327-176.123zm-151.579 144.323c-39.701 0-72-32.299-72-72s32.299-72 72-72 72 32.299 72 72-32.298 72-72 72z"/>
            </g>
          </svg>
          <p>Sélectionner votre adresse de livraison</p>
        </div>

        <div class="Product-description">
          <h1>Description du produit</h1>
          <article class="description">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed aliquam dui tortor, quis semper justo fringilla
            ut. Fusce maximus enim elementum mi tincidunt posuere. Sed pellentesque purus ex, porta aliquam leo
            scelerisque nec. Etiam dignissim nisi ed pellentesque purus ex, porta aliquam leo scelerisque nec.
          </article>
          <center>
            <p class="read-more">Lire plus</p>
            <svg version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
                 x="0px" y="0px" width="14" height="14" viewBox="0 0 123.959 123.958"
                 style="enable-background:new 0 0 123.959 123.958;" xml:space="preserve">
<g>
	<path
    d="M117.979,28.017h-112c-5.3,0-8,6.4-4.2,10.2l56,56c2.3,2.3,6.1,2.3,8.401,0l56-56   C125.979,34.417,123.279,28.017,117.979,28.017z"/>
</g>
</svg>
          </center>
        </div>
      </div>

      <div class="Payment-card">
        <div class="payement-price">
          <p class="price-tilte">Prix originale</p>
          <p class="price-barre">79,99€</p>
        </div>

        <div class="payement-price">
          <p class="price-tilte">Vous économisez</p>
          <p class="price-ok">14,09€</p>
        </div>

        <div class="payement-price">
          <p class="price-tilte">Livraison</p>
          <p class="price-delivery">GRATUITE</p>
        </div>

        <div class="payement-price">
          <p class="price-tilte-total">Total (ttc)</p>
          <p class="price-total">65,90€</p>
        </div>

        <div class="group-button-price">
          <button
            class="p-4 hover:bg-blue-700 text-white font-bold py-2 px-4 border rounded add-cart">
            Ajouter au panier
          </button>
          <button
            class="bg-transparent font-semibold hover:text-white py-2 px-4 buy-now rounded">
            Acheter maintenant
          </button>
        </div>

        <hr data-v-f537270a="" class="border-divider"
            style="margin: 20px auto 0px; width: 95%; border: 1px solid rgb(120, 120, 120); border-radius: 5px;">

        <div class="fois-four">
          <center>
            <p class="price-tilte">Ou payez en 4x</p>
            <p class="price-tilte">16,48 € (+ 2,18€ de frais)</p>
          </center>
        </div>
      </div>
    </div>
    <completely/>
    <productcharacteristics/>
    <customeropinion/>
  </section>
</template>

<script>
import completely from '/components/page3/Completely.vue'
import productcharacteristics from '/components/page3/Productcharacteristics.vue'
import customeropinion from '/components/page3/Customeropinion.vue'
export default {
  components: {completely, productcharacteristics, customeropinion},
  data() {
    return {
      favorited: false,
      animating: false
    };
  },
  computed: {
    iconClasses() {
      return {
        "toggle-favorite__icon--favorited": this.favorited,
        "toggle-favorite__icon--animate": this.animating
      };
    }
  },
  methods: {
    toggle() {
      // Only animate on favoriting.
      if (!this.favorited) {
        this.animating = true;
      }

      this.favorited = !this.favorited;
    },
    onIconAnimationEnds() {
      this.animating = false;
    }
  }
}
</script>

<style lang="scss">
@import "assets/scss/variables";

.section-oneProduct {
  display: flex;
  flex-wrap: wrap;
  margin: 3rem 1rem;
  width: 1403px;
  height: 473px;

  .box-picture {
    width: 58px;
    height: 58px;
    margin: 1rem;
    border: 1px solid black;
  }

  .picture-principal {
    display: flex;
    align-items: center;
    justify-content: center;
    border: 1px solid black;
    width: 425px;
    height: 425px;

    .cercle {
      position: relative;
      top: 12rem;
      left: 8rem;
      width: 60px;
      height: 60px;
      border-radius: 51px;
      border: 1px solid black;
      background: white;
      box-shadow: 1px 1px 1px;

      .heart {
        margin-left: 0.9rem;
        margin-right: 1rem;
        margin-top: 1rem;
      }
    }

    @keyframes favorite-icon-animation {
      0% {
        opacity: 1;
        transform: scale(0.1);
      }

      50% {
        opacity: 1;
        transform: scale(1.1);
      }

      80% {
        opacity: 1;
        transform: scale(0.9);
      }

      100% {
        opacity: 1;
        transform: scale(1);
      }
    }

    @keyframes favorite-particles-animation {
      0% {
        background-position: left center;
      }
      100% {
        background-position: right center;
      }
    }

    // Particles animation.
    .favorite-particles-transition-enter-active {
      background-image: url("~/assets/images/animation-like-heart.png");
      background-size: 2500% auto;
      background-position: left center;
      background-repeat: no-repeat;

      animation-duration: $particles-animation-duration;
      animation-timing-function: steps(24);
      animation-name: favorite-particles-animation;
    }

    .toggle-favorite {
      font-size: 20px;
      position: relative;

      &__icon {
        // Transition mainly for when un-favoriting
        transition: fill-opacity 0.2s, stroke 0.2s;
        fill: $icon-color;
        fill-opacity: 0;
        stroke: $icon-border-color;

        &--favorited {
          fill-opacity: 1;
          stroke: $icon-color;
        }

        // Icon animation
        &--animate {
          opacity: 0;
          transform: scale(0);
          animation-duration: $icon-animation-duration;
          animation-delay: $particles-animation-duration - $icon-animation-duration;
          animation-name: favorite-icon-animation;
        }
      }

      &__particles {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 3em;
        height: 3em;
      }
    }
  }

  .description-principal {
    width: 425px;
    height: 425px;
    border: 1px solid black;
    margin-left: 2rem;
    padding: 1rem;

    h1 {
      font-family: Rambla, serif;
      font-weight: bold;
      font-size: 26px;
    }

    .group-stars {
      display: flex;
      margin: 0.5rem;
    }

    .avis-product {
      font-family: Rambla, serif;
      font-size: 13px;
      color: #777777;
    }

    .share {
      margin-left: 11rem;
    }

    .stock {
      font-family: Rambla, serif;
      font-size: 20px;
      color: #ff9a24;
    }

    .free-delivery {
      font-size: 17px;
      font-family: Rambla, serif;
      color: black !important;
    }

    .select-adress {
      display: flex;
      font-size: 12px;
      margin-top: 0.5rem;

    }

  }

  .Product-description {
    margin: 1rem;
    font-size: 20px;

    .description {
      overflow: hidden;
      text-overflow: ellipsis;
      white-space: nowrap;
      font-size: 16px;
      font-family: Rambla, serif;
    }

    .read-more {
      margin-top: 0.5rem;
      font-family: Rambla, serif;
      font-size: 11px;
    }

  }

  .Payment-card {
    border: 1px solid #e1e1e1;
    width: 273px;
    height: 425px;
    margin-left: 4rem;
    padding: 1rem;

    .payement-price {
      display: flex;
      justify-content: space-between;
      margin-top: 0.5rem;

      .price-ok {
        color: #e61010;
      }

      .price-delivery {
        color: #e61010;
        font-size: 0.8rem;
      }

      .price-tilte-total {
        font-family: Rambla, serif;
        font-weight: bold;
        font-size: 1.3rem;
      }

      .price-total {
        font-family: Rambla, serif;
        font-weight: bold;
      }


    }

    .price-tilte {
      font-family: Rambla, serif;
    }

    .price-barre {
      font-family: Rambla, serif;
      text-decoration: line-through;
    }

    .group-button-price {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-content: center;
      margin-top: 1rem;

      .add-cart {
        padding: 0.5rem;
        width: 233px;
        height: 40px;
        background: #ff9a24;
        border: #ff9a24;
      }

      .buy-now {
        padding: 0.5rem;
        width: 233px;
        height: 40px;
        margin-top: 1rem;
        border: 1px solid #ff9a24;
        color: #ff9a24;
      }

      .buy-now:hover {
        background: #ff9a24;
        color: white;

      }
    }

    .fois-four {
      padding: 1rem;
      margin-top: 1.5rem;
      font-weight: bold;
      color: #787878;

    }
  }

}

</style>


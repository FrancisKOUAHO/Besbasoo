<template>
  <div>
    <link rel="stylesheet" href="https://pro.fontawesome.com/releases/v5.10.0/css/all.css"
          integrity="sha384-AYmEC3Yw5cVb3ZcuHtOA93w35dYTsvhLPVnYs9eStHfGJvOvKxVfELGroGkvsg+p" crossorigin="anonymous"/>


    <div class="min-h-screen min-w-screen flex items-center justify-center bg-gray-200 mobile-view-bg-color">
      <br/><br/><br/><br/>
      <div class="flex flex-col">
        <div class="py-6 px-8 text-left">
          <nuxt-link to="/">
            <h1 class="text-center mobile-text-color besbasoo">Besbasoo</h1>
          </nuxt-link>
          <br/>
          <h2 class="text-left  mt-1.5 mobile-text-color vous-e-n">S'identifier<br/></h2>
          <div class="mt-3">
          <span class="text-black text-left font-medium mobile-text-color"
                style="font-family: Rambla;font-size: 18px;font-style: normal;font-weight: 400;line-height: 22px;letter-spacing: 0em;text-align: left;">
            Adresse e-mail ou numéro de téléphone portable
          </span>
          </div>
        </div>
        <form @submit.prevent="handleLogin">
          <div class="flex flex-col  px-8 space-y-5 bg-gray-275">
            <div class="flex flex-wrap items-stretch w-full relative h-15 bg-white items-center rounded pr-10">
              <div class="flex -mr-px justify-center w-12 p-4">
                <span
                  class="flex items-center leading-normal bg-white px-3 border-0 rounded rounded-r-none text-2xl text-gray-600">
                  <i class="fal fa-envelope"></i>
                </span>
              </div>
              <input
                type="email"
                class="flex-shrink flex-grow flex-auto leading-normal w-px flex-1 border-0 h-10 border-grey-light rounded rounded-l-none px-3 self-center relative  font-roboto text-xl outline-none"
                placeholder="Address e-mail"
                v-model="email"
                required
              />
            </div>
            <div
              class="flex flex-wrap items-stretch w-full mb-4 relative h-15 bg-white items-center rounded mb-6 pr-10">
              <div class="flex -mr-px justify-center w-12 p-4">
              <span
                class="flex items-center leading-normal bg-white px-3 border-0 rounded rounded-r-none text-2xl text-gray-600"
              >
                <i class="fal fa-lock-alt"></i>
              </span>
              </div>
              <input
                :type="show ? 'password' : 'text'"
                class="flex-shrink flex-grow flex-auto leading-normal w-px flex-1 border-0 h-10 border-grey-light rounded rounded-l-none px-3 self-center relative  font-roboto text-xl outline-none"
                placeholder="Mot de passe"
                v-model="password"
                required
              />
              <div class="flex -mr-px justify-center w-12 p-4">
                  <span @click="show = !show" :class="{'hidden': !show, 'block':show }"
                        class="flex items-center leading-normal bg-white px-3 border-0 rounded rounded-r-none text-2xl text-gray-600">
                    <i class="fas fa-eye"></i>

                 </span>
                <span @click="show = !show" :class="{'block': !show, 'hidden':show }"
                      class="flex items-center leading-normal bg-white px-3 border-0 rounded rounded-r-none text-2xl text-gray-600">
                    <i class="fas fa-eye-slash"></i>

                 </span>
              </div>

            </div>
            <div class="text-right" style="margin-top: 0px !important;">
              <span class="text-black text-lg text-left font-weight-bold mobile-text-color mot-de-p"> Mot de passe oublie ?</span>
            </div>

            <button
              type="submit"
              class="w-full py-3 bg-yellow-500 text-white rounded-md text-sm focus:outline-none focus:ring-2 focus:ring-orange-500 focus:border-transparent shadow-lg mobile-text-color  creer-m-c">
              Connexion
            </button>
            <hr class="border-divider"
                style="margin: 20px auto 0;width:50%; border: 1px solid #787878; border-radius: 5px; "/>


            <h2
              style="font-family: Rambla;font-style: normal;font-weight: bold;font-size: 30px;line-height: 37px;color: #101829;"
              class="text-black text-lg text-left font-weight-bold mobile-text-color">Vous êtes nouveau ?</h2>
            <nuxt-link :to="{name: 'signUp'}">
              <button
                class="border-2 border-gray-600 w-full py-3 bg-gray text-black rounded-md text-sm focus:outline-none focus:ring-2 focus:ring-white-500 focus:border-transparent shadow-lg mobile-text-color se-conn">
                Créer un compte
              </button>
            </nuxt-link>
            <span class="text-black text-left mobile-text-color mobile-text-color"
                  style="font-family: Rambla;font-style: normal;font-weight: normal;font-size: 15px;line-height: 18px;">
        Vous souhaitez en savoir plus sur la gestion de vos données personnelles ? Consultez la<br> politique de confidentialité accessible depuis le tien suivant :<a
              class="mobile-text-color" style="text-decoration: underline;" href="#"> Protection de la vie privée </a>
      </span>
            <!-- desktop footer -->
            <div class="flex flex-wrap justify-between desktop-view footer-text-color">
              <div><a href=""> Protection de <br/> La vie privé</a></div>
              <div><a href="">Conditions générales <br/> de vente</a></div>
              <div><a href="">Conditions d'adhésion au <br/> programme Marketplace</a></div>
              <div><a href="">Mentions <br/>légales</a></div>
              <div class="py-4"><a href="">Cookies</a></div>
            </div>
            <div class="flex justify-between footer-text-color desktop-view ">
              <div></div>
              <div> @2021, Besbasoo.com, Inc. ou ses filiales</div>
              <div></div>
            </div>
            <!-- desktop footer end -->
          </div>
        </form>
      </div>

    </div>
    <!-- mobile  footer -->
    <div class="footer-bg  min-w-screen  mobile-view footer-text-color">
      <div class="flex  flex-col">
        <div class="text-center"><a href="">Protection de La vie privé</a></div>
        <div class="text-center"><a href="">Conditions générales de vente </a></div>
        <div class="text-center"><a href="">Conditions d'adhésion au programme Marketplace</a></div>
        <div class="text-center"><a href="">Mentions légales </a></div>
        <div class="text-center"><a href="">Cookies</a></div>
      </div>
      <!-- mobile  footer end -->
      <div class="flex justify-between">
        <div></div>
        <div> @2021, Besbasoo.com, Inc. ou ses filiales</div>
        <div></div>
      </div>
    </div>

  </div>
</template>
<script>
import axios from "axios"
import env from '../config/env'

export default {
  layout: 'nothing',
  data() {
    return {
      show: true,
      cshow: true,
      success: false,
      error: false,
      email: "",
      password: "",
    }
  },
  head() {
    return {
      title: 'Connexion | Besbasoo',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Ma description personnalisée'
        }
      ]
    }
  }
}
</script>
<style scoped>
@media only screen and (max-width: 600px) {
  .mobile-view {
    display: block;

  }

  .mobile-view-bg-color {
    background-color: #1752A9 !important;
  }

  .footer-bg {
    background-color: #101829;
    padding: 18px;
  }

  .mobile-text-color {
    color: white !important;
  }

  .se-conn {
    border: 2px solid white !important;
  }

  .border-divider {
    border: 1px solid white !important;

  }


}

@media only screen and (min-width: 600px) {
  .mobile-view {
    display: none;
  }

  .mobile-logo {
    display: none;
  }
}


@media only screen and (max-width: 600px) {
  .desktop-view {
    display: none;
  }
}

.footer-text-color {
  color: #787878;
  font-family: Rambla, serif;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 18px;
}

.besbasoo {
  font-family: Rambla, serif;
  font-style: normal;
  font-weight: bold;
  font-size: 45px;
  line-height: 55px;
  color: #101829
}

.vous-e-n {
  font-family: Rambla, serif;
  font-size: 30px;
  font-style: normal;
  font-weight: 700;
  line-height: 37px;
  letter-spacing: 0em;
  text-align: left;
  color: #101829
}

.creer-m-c {
  font-weight: bold;
  font-family: Rambla, serif;
  font-style: normal;
  font-size: 18px;
  line-height: 22px;
}

.se-conn {
  font-family: Rambla, serif;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 22px;
  color: #101829;
}

.mot-de-p {
  font-family: Rambla, serif;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 37px;
  color: #101829;
}


</style>

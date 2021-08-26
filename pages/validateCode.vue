<template>
  <div class="wrapper">
    <div class="form">

      <div class="title">
        <center><img src="~/assets/images/logo-1.png" alt="logo-1" width="80"></center>
      </div>
      <form @submit.prevent="activate" class="form-horizontal">
        <div class="input_wrap">
          <label for="input_text">Veuillez saissir votre email</label>
          <div class="input_field">
            <input v-model="activateAccountCodeEmail.email" type="text" class="input" id="input_text">
          </div>
        </div>
        <div class="input_wrap">
          <label for="input_password">Veuillez saissir votre code de confirmation</label>
          <div class="input_field">
            <input v-model="activateAccountCodeEmail.code" type="password" class="input" id="input_password">
          </div>
        </div>
        <div class="input_wrap">
          <span class="error_msg">Le nom d'utilisateur ou le mot de passe est incorrect. Veuillez réessayer {{ succes }} {{
              error
            }}</span>
          <input type="submit" class="btn enabled" value="Valider">
        </div>
      </form>
    </div>
  </div>
</template>

<script>
import axios from "axios";
import env from "@/config/env";

export default {
  name: "validateCode",
  layout: 'nothing',
  data: function () {
    return {
      succes: "",
      error: "",
      activateAccountCodeEmail: {
        email: "",
        code: "",
      }
    }
  },
  methods: {
    async activate() {
      try {
        let activateAccount = await axios.patch(`${env.BaseURL}users/activate`, this.activateAccountCodeEmail);
        console.log(activateAccount)
        this.succes = this.activateAccountCodeEmail.success
        await this.$router.push({name: 'index'});
      } catch (e) {
        this.error = this.activateAccountCodeEmail.success
      }
    }
  },
  head() {
    return {
      title: 'Validation Code| Besbasoo',
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
.wrapper {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #1752a9;
}

.form {
  width: 50%;
  height: auto;
  background: #fff;
  padding: 35px 50px;
  border-radius: 2px;
}

.form .title {
  text-align: center;
  margin-bottom: 20px;
  font-weight: 700;
  font-size: 24px;
}

.form .input_wrap {
  width: 325px;
  position: relative;
  margin: 0 auto 2rem auto;
}

.form .input_wrap:last-child {
  margin-bottom: 0;
}

.form .input_wrap label {
  display: block;
  margin-bottom: 5px;
}

.form .input_wrap input {
  padding: 15px;
  width: 100%;
  border: 1px solid transparent;
  font-size: 16px;
  border-radius: 3px;
}

.form .input_wrap .input {
  background: #f5f4f4;
  padding-right: 35px;
}


.form .input_wrap .input:focus {
  border-color: #f59e0b;
}

.form .input_wrap .input_field {
  position: relative;
}

.form .input_wrap .btn {
  text-transform: uppercase;
  letter-spacing: 3px;
  color: #fff;
}

.form .input_wrap .btn.disabled {
  background: #f59e0b;
}

.form .input_wrap .btn.enabled {
  background: #f59e0b;
  cursor: pointer;
}

.form .input_wrap .error_msg {
  font-size: 15px;
  margin-bottom: 5px;
  color: #f74040;
  display: none;
}
</style>

<template>
  <article class="card">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.11.2/css/all.min.css">
    <div class="container">
      <div class="card-title">
        <h2>
          Sélectionnez un mode de paiement
        </h2>
      </div>
      <div class="card-body">
        <div class="payment-type">
          <h4>Plus d'options de paiement</h4>
          <div class="types flex justify-space-between">
            <div class="type selected">
              <div class="logo">
                <i class="far fa-credit-card"></i>
              </div>
              <div class="text">
                <p>Payer par carte de crédit</p>
              </div>
            </div>
            <div class="type">
              <div class="logo">
                <i class="fab fa-paypal"></i>
              </div>
              <div class="text">
                <p>Payez avec PayPal</p>
              </div>
            </div>
            <div class="type">
              <div class="logo">
                <i class="fab fa-amazon"></i>
              </div>
              <div class="text">
                <p>Payer avec Amazon</p>
              </div>
            </div>
          </div>
        </div>
        <br>
        <div class="payment-info flex justify-space-between">
          <div class="column billing">
            <div class="title">
              <div class="num">1</div>
              <h4>Informations sur la facturation</h4>
            </div>
            <br>
            <div class="field full">
              <label for="name">Nom complet</label>
              <input id="name" type="text" placeholder="Nom complet">
            </div>
            <div class="field full">
              <label for="address">Adresse de facturation</label>
              <input id="address" type="text" placeholder="Adresse de facturation">
            </div>
            <div class="flex justify-space-between">
              <div class="field half">
                <label for="city">Ville</label>
                <input id="city" type="text" placeholder="Ville">
              </div>
              <div class="field half">
                <label for="state">État</label>
                <input id="state" type="text" placeholder="État">
              </div>
            </div>
            <div class="field full">
              <label for="zip">Code postale</label>
              <input id="zip" type="text" placeholder="Code postale">
            </div>
          </div>
          <div class="column shipping">
            <div class="title">
              <div class="num">2</div>
              <h4>Informations sur la carte de crédit</h4>
            </div>
            <br>
            <div class="field full">
              <label for="name">Nom du titulaire de la carte</label>
              <input  type="text" placeholder="Nom complet">
            </div>
            <div class="field full">
              <label for="address">Numéro de la carte</label>
              <input  type="text" placeholder="1234-5678-9012-3456">
            </div>
            <div class="flex justify-space-between">
              <div class="field half">
                <label for="city">Exp. Mois</label>
                <input  type="text" placeholder="12">
              </div>
              <div class="field half">
                <label for="state">Année Exp.</label>
                <input  type="text" placeholder="19">
              </div>
            </div>
            <div class="field full">
              <label for="zip">Numéro CVC</label>
              <input  type="text" placeholder="468">
            </div>
          </div>
        </div>
      </div>
      <div class="card-actions flex justify-space-between">
        <div class="flex-start">
          <button class="button button-secondary">Retour au magasin</button>
        </div>
        <div class="flex-end">
          <button class="button button-primary">Procédez au payement </button>
        </div>
      </div>
    </div>
  </article>
</template>

<script>
export default {
  name: "selectPayment",
  head() {
    return {
      title: 'Mode de paiement | Besbasoo',
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
.field {
  margin-bottom: 25px;
}
.field.full {
  width: 100%;
}
.field.half {
  width: calc(50% - 12px);
}
.field label {
  display: block;
  text-transform: uppercase;
  font-size: 12px;
  margin-bottom: 8px;
}
.field input {
  padding: 12px;
  border-radius: 6px;
  border: 2px solid #e8ebed;
  display: block;
  font-size: 14px;
  width: 100%;
  box-sizing: border-box;
}
.field input::placeholder {
  color: #e8ebed !important;
}
.flex {
  display: flex;
  flex-direction: row;
  align-items: center;
}
.flex.justify-space-between {
  justify-content: space-between;
}
.card {
  padding: 50px;
  margin: 50px auto;
  background: #fff;
  border-radius: 6px;
  box-sizing: border-box;
}
.card .container {
  max-width: 700px;
  margin: 0 auto;
}
.card .card-title {
  margin-bottom: 50px;
}
.card .card-title h2 {
  margin: 0;
}
.card .card-body .payment-type,
.card .card-body .payment-info {
  margin-bottom: 25px;
}
.card .card-body .payment-type h4 {
  margin: 0;
}
.card .card-body .payment-type .types {
  margin: 25px 0;
}
.card .card-body .payment-type .types .type {
  width: 30%;
  position: relative;
  background: #f2f4f7;
  border: 2px solid #e8ebed;
  padding: 25px;
  box-sizing: border-box;
  border-radius: 6px;
  cursor: pointer;
  text-align: center;
  transition: all 0.5s ease;
}
.card .card-body .payment-type .types .type:hover {
  border-color: #28333b;
}
.card .card-body .payment-type .types .type:hover .logo,
.card .card-body .payment-type .types .type:hover p {
  color: #28333b;
}
.card .card-body .payment-type .types .type.selected {
  border-color: #ff9a24;
  background: rgba(64,179,255,0.1);
}
.card .card-body .payment-type .types .type.selected .logo {
  color: #ff9a24;
}
.card .card-body .payment-type .types .type.selected p {
  color: #28333b;
}
.card .card-body .payment-type .types .type.selected::after {
  content: '\f00c';
  font-family: 'Font Awesome 5 Free',serif;
  font-weight: 900;
  position: absolute;
  height: 40px;
  width: 40px;
  top: -21px;
  right: -21px;
  background: #fff;
  border: 2px solid #ff9a24;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.card .card-body .payment-type .types .type .logo,
.card .card-body .payment-type .types .type p {
  transition: all 0.5s ease;
}
.card .card-body .payment-type .types .type .logo {
  font-size: 48px;
  color: #8a959c;
}
.card .card-body .payment-type .types .type p {
  margin-bottom: 0;
  font-size: 10px;
  text-transform: uppercase;
  font-weight: 600;
  letter-spacing: 0.5px;
  color: #8a959c;
}
.card .card-body .payment-info .column {
  width: calc(50% - 25px);
}
.card .card-body .payment-info .title {
  display: flex;
  flex-direction: row;
  align-items: center;
}
.card .card-body .payment-info .title .num {
  height: 24px;
  width: 24px;
  border-radius: 50%;
  border: 2px solid #ff9a24;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  margin-right: 12px;
  font-size: 12px;
}
.button {
  text-transform: uppercase;
  font-weight: 600;
  font-size: 12px;
  letter-spacing: 1px;
  padding: 15px 25px;
  border-radius: 5px;
  cursor: pointer;
  transition: all 0.5s ease;
  background: transparent;
  border: 2px solid transparent;
}
.button.button-link {
  padding: 0 0 2px;
  margin: 0 25px;
  border-bottom: 2px solid rgba(64,179,255,0.5);
  border-radius: 0;
  opacity: 0.75;
}
.button.button-link:hover {
  border-bottom: 2px solid #ff9a24;
  opacity: 1;
}
.button.button-primary {
  background: #ff9a24;
  color: #fff;
}
.button.button-primary:hover {
  background: #cb7204;
}
.button.button-secondary {
  background: transparent;
  border-color: #e8ebed;
  color: #8a959c;
}
.button.button-secondary:hover {
  border-color: #28333b;
  color: #28333b;
}


</style>

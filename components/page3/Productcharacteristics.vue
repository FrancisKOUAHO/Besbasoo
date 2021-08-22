<template>
  <div class="Product-characteristics">
    <h1>Caractéristique du produit</h1>
    <table>
      <tbody>
      <tr>
        <td data-label="Account">Taille</td>
        <td data-label="Due Date">60 x 40 CM</td>

      </tr>
      <tr>
        <td data-label="Amount">Marque</td>
        <td data-label="Period">ANZENGRUBER KERAMIK</td>
      </tr>
      <tr>
        <td data-label="Amount">Couleur</td>
        <td data-label="Period">Jaune, multicolor</td>
      </tr>
      <tr>
        <td data-label="Amount">Matériau</td>
        <td data-label="Period">Toile</td>
      </tr>
      <tr>
        <td data-label="Amount">Dimensions de l’article L x l x H</td>
        <td data-label="Period">60 x 40 x 2 centimètres</td>
      </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: "Productcharacteristics"
}
</script>

<style lang="scss">
.Product-characteristics {
  width: 95%;
  margin: auto;
  padding: 1rem;
  font-family: Rambla, serif;

  h1 {
    font-size: 30px;
    font-weight: bold;
  }

  table {
    border: 1px solid #343333;
    border-collapse: collapse;
    color: #777676;
    margin: 0;
    padding: 0;
    width: 100%;
    table-layout: fixed;
  }

  table caption {
    font-size: 1.5em;
    margin: .5em 0 .75em;
  }

  table tr {
    background-color: white;
    border: 1px solid #ddd;
    padding: .35em;
  }

  table th,
  table td {
    padding: 0.625em;
    text-align: left;
  }

  table th {
    font-size: .85em;
    letter-spacing: .1em;
    text-transform: uppercase;
  }

  @media screen and (max-width: 600px) {
    table {
      border: 0;
    }

    table caption {
      font-size: 1.3em;
    }

    table thead {
      border: none;
      clip: rect(0 0 0 0);
      height: 1px;
      margin: -1px;
      overflow: hidden;
      padding: 0;
      position: absolute;
      width: 1px;
    }

    table tr {
      border-bottom: 3px solid white;
      display: block;
      margin-bottom: .625em;
    }

    table td {
      border-bottom: 1px solid #ddd;
      display: block;
      font-size: .8em;
      text-align: right;
    }

    table td::before {
      /*
      * aria-label has no advantage, it won't be read inside a table
      content: attr(aria-label);
      */
      content: attr(data-label);
      float: left;
      font-weight: bold;
      text-transform: uppercase;
    }

    table td:last-child {
      border-bottom: 0;
    }
  }
}

</style>

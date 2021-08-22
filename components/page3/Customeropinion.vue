<template>
  <div class="customer-opinion">
    <h1>Avis</h1>
    <div class="group-reviews">
      <div class="customer-opinion-reviews">
        <center>
          <p class="vote">4.0</p>
        </center>
        <div class="rating-container">
           <span class="rating-rating" v-for="rating in 4">
              <svg class="mx-1 w-4 h-4 fill-current text-yellow-500" xmlns="http://www.w3.org/2000/svg"
                   viewBox="0 0 20 20">
                <path
                    d="M10 15l-5.878 3.09 1.123-6.545L.489 6.91l6.572-.955L10 0l2.939 5.955 6.572.955-4.756 4.635 1.123 6.545z"/>
              </svg>
           </span>

          <span class="rating-rating">
            <svg class="mx-1 w-4 h-4 fill-current text-gray-400" xmlns="http://www.w3.org/2000/svg"
                 viewBox="0 0 20 20">
            <path
                d="M10 15l-5.878 3.09 1.123-6.545L.489 6.91l6.572-.955L10 0l2.939 5.955 6.572.955-4.756 4.635 1.123 6.545z"/>
            </svg>
          </span>
        </div>
        <p class="customer-review">46 avis</p>
        <button
            class="p-4 hover:bg-blue-700 text-white font-bold py-2 px-4 border rounded comment">
          Rédiger un commentaire
        </button>
      </div>

      <div class="customer-reviews">
        <div class="customer-reviews-name">
          <div>
            <svg version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
                 x="0px" y="0px" width="30" height="30" viewBox="0 0 53 53" style="enable-background:new 0 0 53 53;"
                 xml:space="preserve">
<path style="fill:#E7ECED;"
      d="M18.613,41.552l-7.907,4.313c-0.464,0.253-0.881,0.564-1.269,0.903C14.047,50.655,19.998,53,26.5,53  c6.454,0,12.367-2.31,16.964-6.144c-0.424-0.358-0.884-0.68-1.394-0.934l-8.467-4.233c-1.094-0.547-1.785-1.665-1.785-2.888v-3.322  c0.238-0.271,0.51-0.619,0.801-1.03c1.154-1.63,2.027-3.423,2.632-5.304c1.086-0.335,1.886-1.338,1.886-2.53v-3.546  c0-0.78-0.347-1.477-0.886-1.965v-5.126c0,0,1.053-7.977-9.75-7.977s-9.75,7.977-9.75,7.977v5.126  c-0.54,0.488-0.886,1.185-0.886,1.965v3.546c0,0.934,0.491,1.756,1.226,2.231c0.886,3.857,3.206,6.633,3.206,6.633v3.24  C20.296,39.899,19.65,40.986,18.613,41.552z"/>
              <g>
	<path style="fill:#556080;"
        d="M26.953,0.004C12.32-0.246,0.254,11.414,0.004,26.047C-0.138,34.344,3.56,41.801,9.448,46.76   c0.385-0.336,0.798-0.644,1.257-0.894l7.907-4.313c1.037-0.566,1.683-1.653,1.683-2.835v-3.24c0,0-2.321-2.776-3.206-6.633   c-0.734-0.475-1.226-1.296-1.226-2.231v-3.546c0-0.78,0.347-1.477,0.886-1.965v-5.126c0,0-1.053-7.977,9.75-7.977   s9.75,7.977,9.75,7.977v5.126c0.54,0.488,0.886,1.185,0.886,1.965v3.546c0,1.192-0.8,2.195-1.886,2.53   c-0.605,1.881-1.478,3.674-2.632,5.304c-0.291,0.411-0.563,0.759-0.801,1.03V38.8c0,1.223,0.691,2.342,1.785,2.888l8.467,4.233   c0.508,0.254,0.967,0.575,1.39,0.932c5.71-4.762,9.399-11.882,9.536-19.9C53.246,12.32,41.587,0.254,26.953,0.004z"/>
              </g>
</svg>
          </div>
          <div class="customer-reviews-lastname">
            <p>kouaho78</p>
          </div>
          <div class="customer-reviews-star">
            <span v-for="star in 5">
              <svg class="mx-1 w-4 h-4 fill-current text-yellow-500" xmlns="http://www.w3.org/2000/svg"
                   viewBox="0 0 20 20">
              <path
                  d="M10 15l-5.878 3.09 1.123-6.545L.489 6.91l6.572-.955L10 0l2.939 5.955 6.572.955-4.756 4.635 1.123 6.545z"/>
            </svg>
            </span>
          </div>
        </div>
        <p class="customer-reviews-p">
          Dolor sit amet, consectetur adipiscing elit. Sed aliquam dui tortor, quis semper justo fringilla ut. Fusce
          maximus enim elementum mi tincidunt posuere. Sed pellentesque purus ex, porta aliquam leo scelerisque nec.
          <span class="customer-reviews-span">Afficher plus</span>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Customeropinion"
}
</script>

<style lang="scss">
@import "assets/scss/variables";

.customer-opinion {
  margin: auto;
  padding: 3rem;
  font-family: Rambla, serif;

  h1 {
    font-size: 30px;
    font-weight: bold;
  }

  .group-reviews {
    display: flex;
    justify-content: center;
    margin: 1rem;
    flex-wrap: wrap;

    @media only screen and (max-width: $mobilMediaMinWidth) {
      .group-reviews{
        width: 100%;
      }
    }


    .customer-opinion-reviews {
      display: flex;
      flex-direction: column;
      padding: 1rem;

      .vote {
        font-family: Rambla, serif;
        font-weight: bold;
        font-size: 85px;
      }

      .rating-container {
        margin-right: auto;
        margin-left: auto;
      }

      .rating-rating {
        float: left;
      }
    }

    .customer-reviews {
      padding: 1rem;
      margin-left: 3rem;

      @media only screen and (max-width: $mobilMediaMinWidth) {
        .customer-reviews{
          width: none;
        }
      }

      .customer-reviews-name {
        display: flex;
        flex-wrap: wrap;
        padding: 1rem;
      }

      .customer-reviews-lastname {
        color: black;
        font-family: Rambla, serif;
        font-size: 1.5rem;
        margin-left: 1rem;
      }

      .customer-reviews-star {
        margin-left: 1rem;
        display: flex;
        padding: 0.5rem;
      }

      .customer-reviews-p{
        font-family: Rambla, serif;
        font-size: 0.9rem;

        .customer-reviews-span{
          color: #ff9a24;
        }
      }
    }

  }

  .customer-review {
    font-family: Rambla, serif;
    font-size: 20px;
    margin-right: auto;
    margin-left: auto;
  }

  .comment {
    padding: 0.5rem;
    width: 233px;
    height: 40px;
    margin-top: 1rem;
    border: 1px solid #ff9a24;
    color: #ff9a24;

  }

  .comment:hover {
    background: #ff9a24;
    color: white;
    @media only screen and (max-width: $mobilMediaMinWidth) {
      .comment:hover{
        background: #ff9a24;
        color: white;
      }
    }
  }
}

</style>

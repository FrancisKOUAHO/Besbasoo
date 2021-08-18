<template>
  <div class="customer-opinion">
    <h1>Avis</h1>
    <div class="group-reviews">
      <div class="customer-opinion-reviews">
        <center>
          <p class="vote">4.0</p>
        </center>
        <div  class="rating-container">
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
.customer-opinion {
  width: 1350px;
  height: 387px;
  margin-left: auto;
  margin-right: auto;
  padding: 1rem;
  font-family: Rambla, serif;
  border: 1px solid greenyellow;

  h1 {
    font-size: 30px;
    font-weight: bold;
  }

  .group-reviews {
    display: flex;
    justify-content: center;
    margin: 1rem;


    .customer-opinion-reviews {
      display: flex;
      flex-direction: column;
      border: 1px solid purple;
      width: 287px;
      height: 300px;
      padding: 1rem;

      .vote {
        font-family: Rambla, serif;
        font-weight: bold;
        font-size: 85px;
      }

      .rating-container{
        margin-right: auto;
        margin-left: auto;
      }

      .rating-rating {
        float: left;
      }
    }

    .customer-reviews {
      border: 1px solid greenyellow;
      width: 800px;
      height: 300px;
      padding: 1rem;
      margin-left: 3rem;
    }

  }

  .customer-review{
    font-family: Rambla, serif;
    font-size: 20px;
    margin-right: auto;
    margin-left: auto;
  }

  .comment{
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
  }


}

</style>

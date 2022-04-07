<template>
  <div class ="card-item-container">
      
    <div class="card-item-top">
      <img :src="product.src" class="card-item-image">
    </div>
    <div class="card-item-bottom">
      <h3 class="card-item-title"><b> {{product.title}} </b></h3>
      <p class="card-item-text">{{product.bgtext}}</p>
      <a v-bind:href= product.page>
        <button class="card-item-button" > {{product.button}}  </button>
      </a>
    </div>
  </div>
</template>

<script setup>
export default {
    name: 'post',
    props: ['product'],
    data () {
      return {
        description: 'A card component'
      }
    },
  }


  
</script>

<style >
  .card-item-container {
   display: flex;
   flex-direction: column;
   justify-content: center;
   align-items: center;
   gap: 1rem;
}
.card-item-bottom {
  padding: 1rem;
  gap: 1rem;
}
.card-item-top {
  height: 80%;
}

.card-item-bottom a {
  text-decoration: none;
}

.card-item-button {
  display: block;
  width: 100%;
}
.card-item-title {
font-size: 20px;


}
button {

background-color: white;
border-radius: 10px;
width:20px;

}

</style>
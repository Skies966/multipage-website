<template>
  <div class="card-container-body">
    <div class="products-area">
      <h1>Lorem, ipsum dolor.</h1>
    </div>
    <div class="card-container">
      <CardContainerContent v-for="x in products" :key="x.id" :product="x"
      >
      {{x}}
      </CardContainerContent>

    </div>
    <div class="products-area-logo">
      <img src="" alt="">
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, ullam?</p>
    </div>
  </div>
</template>

<script setup>
// Place content here
 export default {
    data () {
      return {
      products: [
      {
        title: 'Lorem, ipsumsssssssssssssssssssssssssssssssssssssssssssssssss.',
        button: 'Lorem, ipsumasaaaaaaas.',
        bgtext: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, ullam?sss',
        src: require('../../assets/images/snake1.jpg'),
      },
      {
        title: 'Lorem, ipsumsssssssssssssssssssssssssssssssssssssssssssssssss.',
        button: 'Lorem, ipsumasaaaaaaas.',
        bgtext: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, ullam?sss',
        src: require('../../assets/images/snake1.jpg'),
      }
    ]}
  }}
</script>

<style>


.card-container-body {
  display:flex;
  flex-direction: column;
  align-items: center;
  justify-items: center;
  text-align: center;
  gap: 1rem;

  background-color: rgba(128, 128, 128, 0.555);
  text-shadow: 3px 6px 4px rgba(0, 0, 0, 0.15);
  height: 100%;
  position: relative;
}
 .card-container {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
gap: 1.5rem;
border: 1rem;
font : 5rem;

}

.products-area-logo {
width: 100px;
}


</style>
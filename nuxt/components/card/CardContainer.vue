<template>
  <div class="card-container-body">
    <div class="products-area">
      <h1>Lorem, ipsum dolor.</h1>
    </div>
    <div class="card-container">
      <CardContainerContent 
        :title="products[0].title"
        :bgtext ="products[0].bgtext"
        :src ="products[0].src"
        :button ="products[0].button"  
      >
      </CardContainerContent>
    </div>
    <div class="products-area-logo">
      <img src="" alt="">
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, ullam?</p>
    </div>
  </div>
</template>

<script setup>

const products = ([

        {
          title: 'Lorem, ipsum.',
          button: 'Lorem, ipsum.',
          bgtext: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, ullam?',
          src: require('../../assets/images/snake1.jpg'),
        },
        {
          title: 'Lorem, ipsum.',
          button: 'Lorem, ipsum.',
          bgtext: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, ullam?',
          src: require('../../assets/images/snake1.jpg'),
        },
        {
          title: 'Lorem, ipsum.',
          button: 'Lorem, ipsum.',
          bgtext: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, ullam?',
          src: require('../../assets/images/snake1.jpg'),
        },
        {
          title: 'Lorem, ipsum.',
          button: 'Lorem, ipsum.',
          bgtext: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, ullam?',
          src: require('../../assets/images/snake1.jpg'),
        }
])
</script>

<style>


.card-container-body {
  display:flex;
  flex-direction: column;
  align-items: center;
  justify-items: center;
  text-align: center;
  gap: 1rem;

  background-color: grey;
  text-shadow: 3px 6px 4px rgba(0, 0, 0, 0.15);
  height: 100%;
  position: relative;
}
 .card-container {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
gap: 1.5rem;
border: 1rem;

}

.products-area-logo {
width: 100px;
}


</style>
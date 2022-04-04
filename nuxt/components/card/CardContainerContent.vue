<template>
  <div class ="card-item-container">
    <div class="card-item-top">
      <img :src="props.src" class="card-item-image">
    </div>
    <div class="card-item-bottom">
      <h3 class="card-item-title"> {{props.title}}</h3>
      <p class="card-item-text">{{props.bgtext}}</p>
      <a href="#" target="_blank">
        <button class="card-item-button"> {{props.button}}  </button>
      </a>
    </div>
  </div>
</template>

<script setup>

  const props = ({
  title: String,
  button: String, //InputEvent
  bgtext: String,
  src: Object,
})


  
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


</style>
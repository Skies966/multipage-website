<template>
  <div>
    <div class="HeroContentContainer">
      <div class="HeroText">
          <img src="" alt=""> <!-- Image -->
          <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea, nemo!</p> <!-- Hero Text -->
          <button> CTA button</button> <!-- CTA Button -->
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style>

.HeroContentContainer {
background-image: url("");
display: flex;
justify-content: start;
align-items: center;
text-align: center;
width: 100%;
}

.HeroText {
  margin-left: 20%;
  width: 25%;
}

.HeroText button {
background-color: blue;
}


.HeroText p {
  color: blue;
}
</style>
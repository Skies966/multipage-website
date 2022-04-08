<template>
  <div>
    <TheHeader>
    </TheHeader>
    <div class="group">

    <div class="jason">
      <h3 class="about-name"> Jason Yeske </h3>
      <img src="../assets/images/jason-yeske.jpg" class="jason-pic">
    </div>

    <div class="hyeju">
      <h3 class="about-name">Hyeju Hong</h3>
      <img src="../assets/images/hyeju.jpg" class="hyeju-pic">

    </div>
      <div class="erik">
      <h3 class="about-name">Erik Parlo</h3>
      <img src="../assets/images/erik.png" class="erik-pic">
    </div>

    <div class="edgar">
      <h3 class="about-name">Edgar Caballero</h3>
      <img src="../assets/images/edgar.jpg" class="edgar-pic">
    </div>
    
    
    
    </div>
    <TheFooter>
    </TheFooter>
  </div>
</template>

<<<<<<< HEAD
<script setup>
=======
<script>

export default {
  name: 'AboutPage',
}

>>>>>>> e481f5402c4da905148e7fef870a8628cf338b4a

</script>

<style>
.group {

padding:2px;
text-align: center;
display:flex;
justify-content:space-between;


}
.jason, .hyeju, .erik, .edgar {
border:2px solid black;
}

.jason-pic  {
  width:250px;
  margin-left: auto;
  margin-right:auto;
}
.hyeju-pic  {
  width:250px;
  height:250px;
  margin-left: auto;
  margin-right:auto;
}
.erik-pic  {
  width:250px;
  margin-left: auto;
  margin-right:auto;
}

.edgar-pic {
  /* If you want my huge face */
  /* object-fit: cover */
  object-fit: contain; 
  width:250px;
  height: 250px;
  margin-left: auto;
  margin-right:auto;
  background-color: black;
}
.about-name {
  font-size: 25px;
}


</style>
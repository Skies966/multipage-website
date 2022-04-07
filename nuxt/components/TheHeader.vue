<template>
  <div>
    <nav class="navbar">
      <div class="brand-title">
          <NuxtLink to="/" class="brand-title-item"> Vibrance 
          <img src="../assets/images/gw-logo.svg" alt="Vibrance Logo"></NuxtLink>
          
      </div>
      <div class="navbar-links">
        <ul>
          <NuxtLink to="/about"> About </NuxtLink>
          <NuxtLink to="/animal"> Animals </NuxtLink>
          <NuxtLink to="/environment"> Environment </NuxtLink>

        </ul>
      </div>
    </nav>
  </div>
</template>

<script>

</script>

<style >

  /* Navbar styles  */
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: lightgrey;
    color: black;

  }

  .brand-title {
    display: block;
  }
  .brand-title-item {
    display: flex;
  }

  .brand-title img {
    width: 100%;
    max-width: 50px;
  }

  .navbar-links {
    margin-right: 5%;
  }
  .navbar-links ul{
    margin: 0;
    padding: 0;
    display: flex;
  }

  .navbar-links li {
    list-style: none;
    
  }

  .navbar-links a {
    text-decoration: none;
    color: white;
    padding:5px;
  }
  /* Hover  */
  .navbar-links a:hover{
    color: blue;
  }


</style>
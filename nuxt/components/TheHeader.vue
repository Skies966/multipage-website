<template>
  <div>
    <nav class="navbar">
      <div class="brand-title">
          <p>Lorem</p>
          <img src="" alt="">
      </div>
      <div class="navbar-links">
        <ul>
          <li><a href="#">About</a></li>
          <li><a href="#">Support</a></li>
          <li><a href="#">History</a></li>
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
    background-color: black;
    color: white;

  }

  .brand-title {
    display: block;
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

  .navbar-links li a {
    text-decoration: none;
    color: white;
  }
  /* Hover  */
  .navbar-links li a:hover{
    color: blue;
  }

</style>
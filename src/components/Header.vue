<template>
  <nav id="main-navbar" class="navbar">
    <div class="container navbar-content">
      <!-- <img src="../images/thorlogopng1.png" alt=""> <a class="navbar-brand" href="#">
        <img src="../assets/images/logoskiname8.svg" alt />
      </a>-->
      <router-link to="/"
       class="navbar-brand" href="#">
        <img src="../assets/images/logoskiname8.svg" alt />
      </router-link>

      <!-- <div >   class="nav-items"-->
        <div id="nav" >
          <router-link to="/" class="nav-items">Home</router-link>
          <router-link to="/about" class="nav-items">About</router-link>
          <router-link to="/products" class="nav-items">Products</router-link>
          <router-link to="/contact" class="nav-items">Contact</router-link>

          <router-link to="/cart" class="nav-items"> <i class="fas fa-shopping-cart"></i> </router-link>

        </div>
      <!-- </div> -->
    </div>
  </nav>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style>

#nav {
  /* padding: 30px; */
  display: flex;
  
}

#nav a {
  font-weight: bold;
  color: #ffffff;
  text-decoration: none;
  /* padding: 0 0.5rem; */
}

#nav a.router-link-exact-active {
  color: #bcb7ff;
}


.navbar {
  background-color: rgb(76, 76, 107);
  color: var(--navbarText);
}
.nav-item {
  color: var(--navbarText);
  margin: 0 0.4em;
}

.navbar-brand {
  /* width: 20%;
  height: 20%; */
  width: 160px;
  /* height: auto; */
}

.nav-link {
  color: var(--navbarText);
}

.brandname {
  font-family: rocketWildness;
}


  .navbar-content{
    display: flex;
    justify-content: space-between;
    padding: 2em 1em;
  }

  .navbar-nav{
    display: flex;
  }


  .nav-items{
    display: flex;
    align-items: center;
    /* padding: 0 1rem; */
    margin: 0 0.5rem;
  }
</style>
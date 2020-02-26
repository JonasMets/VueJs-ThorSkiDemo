<template>
  <div id="app">
    <Header />
    
    <router-view />

  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import Header from "./components/Header";

export default {
  name: "Home",
  components: {
    // HelloWorld
    Header
  }
};
</script>


<style>
/*  här lägger vi de färger som ska användas */
:root{
  --primaryColor:#505C77;
  --primaryColorDarker:#384a74;
  --primaryBackground:#E1E1E1;
  --navbarText:#F9FAFC;
  --footerText:#F9FAFC;
  --black:#000;
  --black-faded:#1b1b1b;
  --darkGrey: #333;
  --mediumGrey: #444;
  --lightGray: #cfcfcf;
  --white: #fff;
  --boneWhite:#F9FAFC;
  --boxShadowPrimaryD: #505C77;
  --boxShadowGrey: rgba(68, 68,68, .5);
}

/* reset av margin och padding, val av box-sizing */
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-size: 14px;
}


.container {
  max-width: 900px;
  margin: auto;
}

.text-center {
  text-align: center;
}

/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
} */

/* #nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #ffffff;
}

#nav a.router-link-exact-active {
  color: #bcb7ff;
} */
</style>

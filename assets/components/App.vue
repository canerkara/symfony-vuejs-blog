<template>
<div>
  <b-container>
    <Navbar/>
    <CategoryNav/>
    <router-view/>
  </b-container>
  <Footer/>
</div>
</template>

<script>
import Navbar from "../components/Navbar"
import CategoryNav from "./CategoryNav"
import Footer from "./Footer"

export default {
  name: "App",
  components:{CategoryNav, Navbar,Footer}
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,700;1,700&family=Roboto:ital@0;1&display=swap');

html, body {
  font-family: 'Roboto', sans-serif;
}
h1, h2, h3, h4, h5, h6 {
  font-family: "Montserrat",sans-serif;
}

.display-4 {
  font-size: 2.5rem;
}
@media (min-width: 768px) {
  .display-4 {
    font-size: 3rem;
  }
}
.flex-auto {
  flex: 0 0 auto;
}

.h-250 { height: 250px; }
@media (min-width: 768px) {
  .h-md-250 { height: 250px; }
}
</style>
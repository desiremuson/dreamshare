<template>
  <v-app>
    <v-main>
      <Header />
      <Home />
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
import Home from './components/Home'
import Header from './components/Header'
import Footer from './components/Footer'

export default {
  name: 'App',

  components: {
    Home,
    Header,
    Footer
  },

  data: () => ({
    //
  })
}
</script>
<style scoped>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
html {
  font-size: 10px;
  font-family: "Montserrat", sans-serif;
  scroll-behavior: smooth;
}
a {
  text-decoration: none;
}

/* img {
  height: 100%;
  width: 100%;
  object-fit: cover;
}
p {
  color: black;
  font-size: 1.4rem;
  margin-top: 5px;
  line-height: 2.5rem;
  font-weight: 300;
  letter-spacing: 0.05rem;
}

.cta:hover {
  color: white;
  background-color: crimson;
} */
</style>

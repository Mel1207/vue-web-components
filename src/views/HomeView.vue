<template>
  <Navbar />
  <div class="home">
    <h1>hey this is Home</h1>
    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Corporis recusandae ullam illum error</p>
  </div>
  <NavLinks />
</template>

<script>
import Navbar from '../components/Navbar/Navbar.vue'
import NavLinks from '../components/Navbar/NavLinks.vue'

export default {
  name: 'HomeView',
  components: { Navbar, NavLinks },
  setup() {
    console.log('hey mel')

    return {
    }
  }
}
</script>

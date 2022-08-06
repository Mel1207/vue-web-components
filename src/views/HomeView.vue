<template>
  <Navbar />
  <Header />
  <div class="container">
    <h1>hey this is Home</h1>
    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Corporis recusandae ullam illum error</p>
  </div>
</template>

<script>
import Header from '../components/Header/Header.vue'
import Navbar from '../components/Navbar/Navbar.vue'

export default {
  name: 'HomeView',
  components: { Navbar, Header },
  setup() {
    console.log('hey mel')

    return {
    }
  }
}
</script>

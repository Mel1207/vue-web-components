<template>
  <Navbar />
  <Header />
  <SectionAbout />
</template>

<script>
import Header from '../components/Header/Header.vue'
import Navbar from '../components/Navbar/Navbar.vue'
import SectionAbout from '../components/About/SectionAbout.vue'

export default {
  name: 'HomeView',
  components: { Navbar, Header, SectionAbout },
  setup() {
    console.log('hey mel')

    return {
    }
  }
}
</script>

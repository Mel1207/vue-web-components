<template>
  <Navbar />
  <Header />
  <SectionAbout />
  <SectionFeature />
</template>

<script>
import Header from '../components/Header/Header.vue'
import Navbar from '../components/Navbar/Navbar.vue'
import SectionAbout from '../components/Home/SectionAbout.vue'
import SectionFeature from '../components/Home/SectionFeature.vue'


export default {
  name: 'HomeView',
  components: { Navbar, Header, SectionAbout, SectionFeature },
  setup() {
    return {}
  }
}
</script>

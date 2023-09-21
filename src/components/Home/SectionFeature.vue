<template>
  <div class="container">
    <h2 style="margin-bottom: 1.5rem">FAQ</h2>
    <Accordion />
    <Tab />
  </div>
</template>

<script>
import Accordion from '../Accordion/Accordion.vue'
import Tab from '../Tabbed/Tab.vue'

export default {
  components: { Accordion, Tab },
  setup() {
  
    return {}
  }
}
</script>
<template>
  <div v-for="item in accItems" :key="item.id" class="accordion-card">
    <div class="acc-title"  @click="item.isOpen = !item.isOpen">{{ item.title }} <span>+</span></div>
    <transition name="fade">
      <div class="acc-message" v-if="item.isOpen">{{ item.message }}</div>
    </transition>
  </div>
</template>

<script>
import { ref } from '@vue/reactivity'
export default {
  components: {},
  setup() {
    const accItems = ref([
      { 
        id: 1,
        title: "Test title 1",
        message: "lorem ipsum dolor sit amet is simply dummy text of the printing and typesetting industry.",
        isOpen: true
      },
      { 
        id: 2,
        title: "Test title 2",
        message: "lorem ipsum dolor sit amet is simply dummy text of the printing and typesetting industry.",
        isOpen: false
      },
      { 
        id: 3,
        title: "Test title 3",
        message: "lorem ipsum dolor sit amet is simply dummy text of the printing and typesetting industry.",
        isOpen: false
      }
    ])

    const runConso = (item) => {
      console.log('im running console ' + item.isOpen)
    }

    return { accItems, runConso }
  }

}
</script>

<style>

</style>
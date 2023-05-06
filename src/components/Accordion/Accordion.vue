<template>
  <div v-for="item in accItems" :key="item.id">
    <div class="acc-title">{{ item.title }}</div>
    <div class="acc-message">{{ item.message }}</div>
  </div>
</template>

<script>
export default {
  components: {},
  setup() {
    const accItems = [
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
    ]

    return { accItems }
  }

}
</script>

<style>

</style>
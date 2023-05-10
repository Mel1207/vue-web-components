<template>
  <div v-for="tab in tabItems" :key="tab.id">
    <div class="tabs" @click="selectActiveTab(tab.id)">
      <h1>{{ tab.tabTitle }}</h1>
    </div>
    <div class="tab-content">
      <p v-if="tab.isActive">
        {{ tab.tabContent }}
      </p>
    </div>
  </div>
</template>

<script>
import { ref } from 'vue'
export default {
  components: {},
  setup() {
    const tabItems = ref([
      { 
        id: 1,
        tabTitle: 'Title 1', 
        tabContent: '1 Lorem ipsum dolor, sit amet consectetur adipisicing elit. Et, corrupti lorem.',
        isActive: true
      },
      { 
        id: 2,
        tabTitle: 'Title 2', 
        tabContent: '2 Lorem ipsum dolor, sit amet consectetur adipisicing elit. Et, corrupti. amet consectetur adipisicing elit',
        isActive: false
      },
      { 
        id: 3,
        tabTitle: 'Title 3', 
        tabContent: '3 Lorem ipsum dolor, sit amet consectetur adipisicing elit. Et, corrupti.',
        isActive: false
      }
    ])

    const selectActiveTab = (id) => {
      console.log(`selected tab is ${id}`)
    }


    return { tabItems, selectActiveTab }
  }
}
</script>
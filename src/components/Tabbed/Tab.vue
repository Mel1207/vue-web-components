<template>
  <div v-for="tab in tabItems" :key="tab.id"  @click="selectActiveTab(tab.id)">
    <h1>{{ tab.tabTitle }}</h1>
  </div>

  <div class="tab-content" v-for="content in tabContent" :key="content.id">
    <p v-if="activeTab == 1">
      {{ content[0] }}
    </p>
  </div>
</template>

<script>
import { ref } from 'vue'
export default {
  components: {},
  setup() {
    const activeTab = ref('')

    const tabItems = ref([
      { 
        id: 1, 
        tabTitle: 'Title 1',
        isActive: true
      },
      { 
        id: 2, 
        tabTitle: 'Title 2',
        isActive: true
      },
      { 
        id: 3, 
        tabTitle: 'Title 3',
        isActive: true
      }
    ])
    const tabContent = ref([
      { 
        id: 1,
        tabContent: '1 Lorem ipsum dolor, sit amet consectetur adipisicing elit. Et, corrupti lorem.',
        isActive: true
      },
      { 
        id: 2,
        tabContent: '2 Lorem ipsum dolor, sit amet consectetur adipisicing elit. Et, corrupti. amet consectetur adipisicing elit',
        isActive: false
      },
      { 
        id: 3,
        tabContent: '3 Lorem ipsum dolor, sit amet consectetur adipisicing elit. Et, corrupti.',
        isActive: false
      }
    ])

    const selectActiveTab = (id) => {
      console.log(`selected tab is ${id}`)

      activeTab.value = id
      console.log(activeTab.value)
    }


    return { tabItems, tabContent, selectActiveTab, activeTab }
  }
}
</script>
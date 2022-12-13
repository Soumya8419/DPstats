
<script>
import DemoGrid from './Grid.vue'
import userData from './dp.json'
export default {
  components: {
    DemoGrid
  },
  data: () => ({
    searchQuery: '',
    gridColumns: ['url','name', 'successRate'],
    gridData: userData,
    
  })
}
</script>

<template>
  <h1><b>Flare Top Data Providers</b></h1>
  <form id="search">
    Search <input name="query" v-model="searchQuery">
  </form>
  <DemoGrid
    :data="gridData"
    :columns="gridColumns"
    :filter-key="searchQuery">
  </DemoGrid>
</template>

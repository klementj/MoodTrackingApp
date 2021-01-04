<template>
  <!-- <header class="header">
    <div class="container">
      <div class="battery">

      </div>
    </div>
  </header> -->
  <div class="container justify-between">
    <div>
      <ListEpisodes />
    </div>
    <!-- <AddForm /> -->
    <AddButton class="self-end place-self-end"/>
  </div>
</template>

<script>
import AddButton from './components/atoms/addButton.vue'
import AddForm from './components/molecules/addForm.vue'
import ListEpisodes from './components/templates/listEpisodes.vue'

export default {
  name: 'App',
  components: {
    AddForm,
    ListEpisodes,
    AddButton
  }
}
</script>

<style scoped>
/* .header {
  @apply bg-green-800;
}

.battery {
  @apply h-5 bg-green-50 rounded;
} */

.container {
  @apply max-w-sm p-5 flex flex-col min-h-screen;
}
</style>

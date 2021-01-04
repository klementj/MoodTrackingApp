<template>
  <Emojis />

  <article>
    <!-- <svg>
      <use :xlink:href="`#${rating}`" />
    </svg> -->
    <h1>{{ title }}</h1>
    <p class="date">{{ date }}</p>
    <p>{{ description }}</p>
    <p>Rating: {{ rating }}</p>
 
  </article>
</template>

<script>
import Emojis from "../atoms/emojis.vue"

export default {
  name: 'EpisodeCard',
  props: {
    title: String,
    description: String,
    date: String,
    rating: Number
  },
  components: {
    Emojis
  }
}
</script>

<style scoped>
article {
  @apply bg-white p-5 rounded mb-5;
}

h1 {
  @apply font-bold;
}

.date {
  @apply text-gray-400;
}
</style>
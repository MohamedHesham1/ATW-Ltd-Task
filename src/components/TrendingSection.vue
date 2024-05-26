<template>
  <div>
    <CarouselComponent
      :collections="collections"
      sectionTitle="Trending in Photography"
      :showCategoryButton="true"
      bgColor="bg-[#816797]"
      height="h-[303px]"
    />
  </div>
</template>

<script setup>
import CarouselComponent from './CarouselComponent.vue'

const collections = [
  { id: 1, title: 'Giovani Kososki', image: '/Giovani Kososki.png' },
  {
    id: 2,
    title: 'ArtStation - Explore',

    image: '/ArtStation - Explore.png'
  },
  { id: 3, title: 'Amelia', image: '/Amelia.png' },
  { id: 4, title: 'Amelia', image: '/ArtStation - Explore.png' },
  { id: 5, title: 'Amelia', image: '/Giovani Kososki.png' }
]
</script>

<style scoped></style>

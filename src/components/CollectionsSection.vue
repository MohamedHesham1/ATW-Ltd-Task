<template>
  <div>
    <CarouselComponent
      :collections="collections"
      sectionTitle="Collections"
      :showCategoryButton="false"
      :visibleCards="4"
    />
    <div class="bg-[#816797] opacity-70 w-full h-2"></div>
  </div>
</template>

<script setup>
import CarouselComponent from './CarouselComponent.vue'

const collections = [
  {
    id: 1,
    title: 'XO Girls NFT Collection',
    floor: 'Floor: 0.07 ETH',
    image: '/XO Girls NFT Collection.png'
  },
  {
    id: 2,
    title: 'Game character 3d Collection',
    floor: 'Floor: 0.05 ETH',
    image: '/Game character 3d Collection.png'
  },
  {
    id: 3,
    title: 'Monkey Collections',
    floor: 'Floor: 0.01 ETH',
    image: '/Monkey Collections.png'
  },
  { id: 4, title: 'PROJECT NFT cub', floor: 'Floor : 0.07 ETH', image: '/PROJECT NFT cub.png' },
  {
    id: 5,
    title: 'XO Girls NFT Collection',
    floor: 'Floor: 0.07 ETH',
    image: '/XO Girls NFT Collection.png'
  },
  { id: 6, title: 'Monkey Collections', floor: 'Floor: 0.01 ETH', image: '/Monkey Collections.png' }
]
</script>

<style scoped></style>

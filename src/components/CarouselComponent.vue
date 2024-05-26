<template>
  <section class="bg-black text-white px-2 py-8 md:py-12">
    <div class="container mx-auto">
      <div class="flex flex-wrap justify-between items-center mb-8">
        <h2 class="text-3xl md:text-4xl font-bold mb-4 md:mb-0">{{ sectionTitle }}</h2>
        <button
          v-if="showCategoryButton"
          class="btn rounded-[16px] bg-[#52057B] bg-opacity-70 font-medium text-xl text-white hover:bg-transparent hover:border-[#52057B]"
        >
          {{ categoryButtonText }}
        </button>
      </div>
      <div class="relative">
        <button
          @click="scrollLeft"
          class="absolute flex justify-center items-center w-[69px] h-[69px] left-0 top-1/2 transform -translate-y-1/2 bg-[#52057B] text-white rounded-full z-10 text-3xl"
        >
          <i class="fa-solid fa-angle-left"></i>
        </button>
        <div
          ref="scrollContainer"
          class="flex overflow-x-auto lg:overflow-x-hidden scroll-smooth gap-5 px-4"
        >
          <div
            v-for="item in collections"
            :key="item.id"
            :class="['relative min-w-[314px] bg-black rounded-lg']"
          >
            <img :src="item.image" :alt="item.title" :class="[height, 'rounded-t-lg w-full ']" />
            <div :class="[bgColor, 'absolute bottom-0 text-center bg-opacity-75 p-4 w-full']">
              <h3 class="text-lg font-bold">{{ item.title }}</h3>
              <p class="text-sm">{{ item.floor }}</p>
            </div>
          </div>
        </div>
        <button
          @click="scrollRight"
          class="w-[69px] h-[69px] absolute right-0 top-1/2 transform -translate-y-1/2 bg-[#52057B] text-white rounded-full z-10 text-3xl"
        >
          <i class="fa-solid fa-angle-right"></i>
        </button>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'

const props = defineProps({
  collections: Array,
  height: String,
  sectionTitle: String,
  bgColor: {
    type: String,
    default: 'bg-black'
  },
  showCategoryButton: {
    type: Boolean,
    default: false
  },
  categoryButtonText: {
    type: String,
    default: 'View Category'
  }
})

const scrollContainer = ref(null)

const scrollLeft = () => {
  scrollContainer.value.scrollBy({ left: -300, behavior: 'smooth' })
}

const scrollRight = () => {
  scrollContainer.value.scrollBy({ left: 300, behavior: 'smooth' })
}
</script>

<style scoped></style>

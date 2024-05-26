<template>
  <section>
    <div
      class="flex flex-wrap-reverse gap-10 md:gap-[7.125rem] items-center justify-center text-white p-8 md:p-12"
    >
      <div
        class="flex flex-col items-start max-w-[465px] text-lg md:text-xl lg:text-[2rem] text-left lg:leading-[3rem]"
      >
        <h2>“{{ title }}”</h2>
        <p>{{ text }}</p>
        <p class="font-bold">{{ price }}</p>
        <button
          class="mt-6 btn-ghost p-4 border border-purple-600 text-purple-600 rounded-full flex items-center"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            class="w-6 h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M9 5l7 7-7 7"
            />
          </svg>
        </button>
      </div>

      <div class="flex justify-center w-full md:w-auto">
        <img :src="imagePath" :alt="title" class="w-full h-auto max-w-[561px] object-contain" />
      </div>
    </div>
    <div class="bg-[#816797] opacity-70 w-full h-2"></div>
  </section>
</template>

<script setup>
const props = defineProps({
  imagePath: String,
  title: String,
  price: String,
  text: String
})
</script>

<style scoped></style>

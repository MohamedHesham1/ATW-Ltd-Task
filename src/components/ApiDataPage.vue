<template>
  <div class="container mx-auto py-8 text-black">
    <h1 class="text-3xl font-bold text-white mb-4">Posts</h1>
    <div v-if="loading" class="text-center">Loading...</div>
    <div v-if="!loading && posts.length > 0">
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
        <div v-for="post in paginatedPosts" :key="post.id" class="card bg-white shadow-lg">
          <div class="card-body">
            <h3 class="card-title text-2xl font-bold">{{ post.title }}</h3>
            <p>{{ post.body }}</p>
          </div>
        </div>
      </div>
    </div>
    <div v-if="!loading && error" class="text-center text-red-600">{{ error }}</div>

    <!-- Pagination Controls -->
    <div v-if="!loading && posts.length > 0" class="flex items-center justify-center mt-4">
      <button @click="prevPage" :disabled="currentPage === 1" class="btn btn-secondary mx-2">
        Previous
      </button>
      <span class="px-4 py-2 text-white">Page {{ currentPage }} of {{ totalPages }}</span>
      <button
        @click="nextPage"
        :disabled="currentPage === totalPages"
        class="btn btn-secondary mx-2"
      >
        Next
      </button>
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted, computed } from 'vue'
import axios from 'axios'

const posts = ref([])
const loading = ref(true)
const error = ref('')
const currentPage = ref(1)
const postsPerPage = 6
const fetchPosts = async () => {
  loading.value = true
  try {
    const response = await axios.get('https://jsonplaceholder.typicode.com/posts')
    posts.value = response.data
  } catch (err) {
    error.value = 'Failed to fetch data'
  } finally {
    loading.value = false
  }
}

const paginatedPosts = computed(() => {
  const start = (currentPage.value - 1) * postsPerPage
  const end = start + postsPerPage
  return posts.value.slice(start, end)
})

const totalPages = computed(() => {
  return Math.ceil(posts.value.length / postsPerPage)
})

const nextPage = () => {
  if (currentPage.value < totalPages.value) {
    currentPage.value++
  }
}

const prevPage = () => {
  if (currentPage.value > 1) {
    currentPage.value--
  }
}

onMounted(fetchPosts)
</script>

<style scoped>
.container {
  padding: 1rem;
  max-width: 1200px;
  margin: 0 auto;
}

button:disabled {
  cursor: not-allowed;
  opacity: 1;
  color: white;
}
</style>

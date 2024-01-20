<template>
  <div class="bg-white shadow-md">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex flex-col md:flex-row justify-center py-3">
        <!-- Category Buttons -->
        <button
          class="mx-1 my-1 md:my-0 bg-gray-200 text-gray-700 rounded-full px-6 py-2 text-sm font-medium hover:bg-gray-300 focus:outline-none focus:ring"
          v-for="category in categories"
          :key="category"
          @click="selectCategory(category)"
        >
          {{ category }}
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      categories: ['All', 'Beverage', 'Food'],
      selectedCategory: 'All',
    };
  },
  methods: {
    selectCategory(category) {
      this.selectedCategory = category;
      // Emit an event or update the view based on the selected category
    },
  },
};
</script>

<style scoped>
/* Additional custom styles if needed */
</style>

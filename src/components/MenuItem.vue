<template>
  <div class="max-w-xs md:max-w-sm lg:max-w-md rounded overflow-hidden shadow-md bg-white m-4">
    <img class="w-full" :src="item.image" alt="Food" />
    <div class="px-6 py-4">
      <div class="font-bold text-xl mb-2">{{ item.name }}</div>
      <p class="text-gray-700 text-base mb-4">
        {{ item.description }}
      </p>
      <div class="flex items-center justify-between">
        <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2">{{ item.price }}</span>
        <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
          Add to cart
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['item'],
};
</script>

<style scoped>
/* Additional custom styles if needed */
</style>

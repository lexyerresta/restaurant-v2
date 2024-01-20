<template>
  <div class="bill-summary">
    <h2 class="text-2xl font-semibold mb-4">Bill Summary</h2>
    <div class="border-t border-b border-gray-200 py-2">
      <div class="flex justify-between items-center mb-2">
        <span>Item 1</span>
        <span class="text-gray-600">$10.00</span>
      </div>
      <div class="flex justify-between items-center mb-2">
        <span>Item 2</span>
        <span class="text-gray-600">$15.00</span>
      </div>
      <!-- ... Add more items here ... -->
    </div>
    <div class="flex justify-between mt-2">
      <span class="font-semibold">Total</span>
      <span>$25.00</span>
    </div>
  </div>
</template>

<style scoped>
.bill-summary {
  background-color: #fff;
  border: 1px solid #e2e8f0;
  border-radius: 0.5rem;
  padding: 1rem;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.bill-summary h2 {
  color: #333;
}

.bill-summary .text-gray-600 {
  color: #4a5568;
}

/* Responsive styles */
@media (max-width: 640px) {
  /* Adjust styles for mobile screens */
  .bill-summary {
    padding: 0.75rem; /* Reduce padding for mobile */
  }
  .bill-summary h2 {
    font-size: 1.5rem; /* Decrease font size for mobile */
  }
  .bill-summary .text-gray-600 {
    font-size: 0.875rem; /* Decrease font size for mobile */
  }
}
</style>

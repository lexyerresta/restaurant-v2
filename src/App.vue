<template>
<div class="container mx-auto px-4 sm:px-8 md:px-16 lg:px-20 xl:px-32">
    <CategoryBar />
    <SearchBar />
    <div class="flex flex-wrap">
      <main class="w-full sm:w-1/2 md:w-2/3 lg:w-3/4 xl:w-4/5">
        <!-- Use a loop to render MenuItem components -->
        <MenuItem v-for="item in menuItems" :key="item.id" :item="item" />
      </main>
      <BillSummary class="w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/5" />
    </div>
    <PaymentMethod />
    <FooterActions />
  </div>
</template>

<script>
import CategoryBar from './components/CategoryBar.vue';
import SearchBar from './components/SearchBar.vue';
import MenuItem from './components/MenuItem.vue';
import BillSummary from './components/BillSummary.vue';
import PaymentMethod from './components/PaymentMethod.vue';
import FooterActions from './components/FooterActions.vue';

export default {
  components: {
    CategoryBar,
    SearchBar,
    MenuItem,
    BillSummary,
    PaymentMethod,
    FooterActions
  },
  data() {
  return {
    menuItems: [
      // Beverages
      {
        id: 1,
        category: 'Beverage',
        name: 'Caramel Frappuccino',
        description: 'Caramel syrup with coffee, milk, and whipped cream.',
        price: '$3.95',
        image: 'https://source.unsplash.com/featured/?caramel,frappuccino'
      },
      {
        id: 2,
        category: 'Beverage',
        name: 'Espresso',
        description: 'Strong and bold espresso coffee.',
        price: '$2.50',
        image: 'https://source.unsplash.com/featured/?espresso'
      },
      {
        id: 3,
        category: 'Beverage',
        name: 'Latte',
        description: 'Creamy espresso with steamed milk.',
        price: '$3.50',
        image: 'https://source.unsplash.com/featured/?latte'
      },
      // Foods
      {
        id: 4,
        category: 'Food',
        name: 'Croissant',
        description: 'Buttery and flaky french pastry.',
        price: '$2.95',
        image: 'https://source.unsplash.com/featured/?croissant'
      },
      {
        id: 5,
        category: 'Food',
        name: 'Sandwich',
        description: 'Freshly made ham and cheese sandwich.',
        price: '$5.50',
        image: 'https://source.unsplash.com/featured/?sandwich'
      },
      {
        id: 6,
        category: 'Food',
        name: 'Salad',
        description: 'A healthy assortment of fresh greens.',
        price: '$4.25',
        image: 'https://source.unsplash.com/featured/?salad'
      },
    ],
  };
},
    };
</script>

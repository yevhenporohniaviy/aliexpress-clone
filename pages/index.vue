<template>
  <MainLayout>
    <div id="IndexPage" class="mt-4 max-w-[1200px] mx-auto px-2 ">
      <div class="grid xl:grid-cols-6 lg:grid-cols-5 md:grid-cols-4 sm:grid-cols-3 grid-cols-2 gap-4" v-if="products">
          <div v-for="product in products" :key="product">
              <ProductComponent :product="product"/>
          </div>
      </div>
    </div>
  </MainLayout>
</template>

<script setup>
import MainLayout from '~/layouts/MainLayout.vue';
const products = [
  {
    id: 1,
    title: 'Item 1',
    description: 'This is the description for Item 1',
    url: 'https://picsum.photos/200?random=1',
    price: 1000
  },
  {
    id: 2,
    title: 'Item 2',
    description: 'This is the description for Item 2',
    url: 'https://picsum.photos/200?random=2',
    price: 2000
  },
  {
    id: 3,
    title: 'Item 3',
    description: 'This is the description for Item 3',
    url: 'https://picsum.photos/200?random=3',
    price: 3000
  },
  {
    id: 4,
    title: 'Item 4',
    description: 'This is the description for Item 4',
    url: 'https://picsum.photos/200?random=4',
    price: 4000
  },
  {
    id: 5,
    title: 'Item 5',
    description: 'This is the description for Item 5',
    url: 'https://picsum.photos/200?random=5',
    price: 5000
  },
  {
    id: 6,
    title: 'Item 6',
    description: 'This is the description for Item 6',
    url: 'https://picsum.photos/200?random=6',
    price: 6000
  },
  {
    id: 7,
    title: 'Item 7',
    description: 'This is the description for Item 7',
    url: 'https://picsum.photos/200?random=7',
    price: 7000
  },
  {
    id: 8,
    title: 'Item 8',
    description: 'This is the description for Item 8',
    url: 'https://picsum.photos/200?random=8',
    price: 8000
  },
  {
    id: 9,
    title: 'Item 9',
    description: 'This is the description for Item 9',
    url: 'https://picsum.photos/200?random=9',
    price: 9000
  }

]

</script>
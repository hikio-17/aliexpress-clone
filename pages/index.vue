<template>
   <MainLayout>
      <div id="IndexPage" class="mt-4 max-w-[1200px] mx-auto px-2">
         <div class="grid xl:grid-cols-6 lg:grid-cols-5 md:grid-cols-4 sm:grid-cols-3 grid-cols-2 gap-4">
            <div v-if="products" v-for="product in products" :key="product">
               <ProductComponent :product="product" />
            </div>
         </div>
      </div>
   </MainLayout>
</template>

<script setup>
import MainLayout from '~/layouts/MainLayout.vue'

const products = [
   {
      id: 1,
      title: 'Title 1',
      description: 'This is a decription',
      url: 'https://picsum.photos/id/7/800/800',
      price: 9999
   },
   {
      id: 1,
      title: 'Title 1',
      description: 'This is a decription',
      url: 'https://picsum.photos/id/7/800/800',
      price: 9999
   },
   {
      id: 1,
      title: 'Title 1',
      description: 'This is a decription',
      url: 'https://picsum.photos/id/7/800/800',
      price: 9999
   },
   {
      id: 1,
      title: 'Title 1',
      description: 'This is a decription',
      url: 'https://picsum.photos/id/7/800/800',
      price: 9999
   },
   {
      id: 1,
      title: 'Title 1',
      description: 'This is a decription',
      url: 'https://picsum.photos/id/7/800/800',
      price: 9999
   },
   {
      id: 1,
      title: 'Title 1',
      description: 'This is a decription',
      url: 'https://picsum.photos/id/1/800/800',
      price: 9999
   },
]
</script>

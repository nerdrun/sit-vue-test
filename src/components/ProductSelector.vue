<script setup lang="ts">
import type { Product } from '../types/product';

const products: Product[] = [
  { id: 1, name: 'Laptop', description: 'Powerful performance' },
  { id: 2, name: 'Headphones', description: 'Noise-canceling magic' },
  { id: 3, name: 'Smartphone', description: 'Pixel-perfect display' }
]
</script>

<template>
  <div>
    <h3>Select a Product</h3>
    <ul>
      <li v-for="product in products" :key="product.id">
        <button>{{ product.name }}</button>
      </li>
    </ul>
  </div>
</template>

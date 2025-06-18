<script setup lang="ts">
</script>

<template>
  <div v-if="product" class="product-preview">
    <h3>Product Preview</h3>
    <p><strong>{{ product.name }}</strong></p>
    <p>{{ product.description }}</p>
  </div>
  <div v-else class="product-preview">
    <p>No product selected</p>
  </div>
</template>
<template>
  <v-app style='background:#e5e6e4'>
    <v-content>
      <ProductCard/>
    </v-content>
  </v-app>
</template>

<script>
import ProductCard from './components/ProductCard';

export default {
  name: 'App',
  components: {
    ProductCard
  },
};
</script>

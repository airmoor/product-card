<template>
  <v-card
    class="mx-auto my-3"
    max-width="600" 
  >
    <Slider/>
    <h2 class="text--primary text-center my-2">1 754 600 рублей</h2>
    <h2 class="text-center">Кресло Мисс Фламинго</h2>
    <v-card-subtitle class="text-center pb-0">Miss Flamingo Chair — AP Collection</v-card-subtitle>
    <OrderForm/>
    <Tabs/>
  </v-card>
</template>

<script>
  import Slider from './Slider'
  import Tabs from './Tabs'
  import OrderForm from './OrderForm'

  export default {
    name: 'ProductCard',
    components: {
      Slider,
      Tabs,
      OrderForm
    },
  }
</script>


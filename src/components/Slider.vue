<template>
  <v-carousel :show-arrows="false" cycle height="600">
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    name: 'Slider',
    data () {
      return {
        items: [
          {
            src:require('./../assets/Flamingo-Chair-1.jpg')
          },
          {
            src:require('./../assets/Flamingo-Chair-2.jpg')
          },
          {
            src:require('./../assets/Flamingo-Chair-3.jpg')
          },
          {
            src:require('./../assets/Flamingo-Chair-4.jpg')
          },
        ],
      }
    },
  }
</script>
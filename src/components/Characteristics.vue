<template>
  <v-container class="lighten-5">
    <template v-for="item in items">
        <v-row :key="item">
            <template v-for="n in 2">
                <v-col :key="n">
                    <p v-if="n % 2 === 1" class='my-0 body-1'>
                        {{item.title}}
                    </p>
                    <p v-else class='my-0 body-1'>
                        {{item.value}}
                    </p>
                         
                </v-col>
                <v-responsive
                    v-if="n === 2"
                    :key="`width-${n}`"
                    width="100%"
                ></v-responsive>
            </template>
        </v-row>
    </template>
  </v-container>
</template>

<script>
  export default {
    name: 'Characteristics',
    data() {
        return {
            items: [
                {
                    title: 'Ширина', value: '104 см'
                },
                {
                    title: 'Высота', value: '118 см'
                },
                {
                    title: 'Глубина', value: '93 см'
                },
                {
                    title: 'Материал', value: 'Натуральный мех'
                },
                {
                    title: 'Материал ножек', value: 'Металл'
                },
                {
                    title: 'Чистый вес', value: '33 кг'
                },
                {
                    title: 'Бренд', value: 'AP Collection'
                },
                {
                    title: 'Производство', value: 'Бельгия'
                }
            ]
        }      
    }
  }
</script>
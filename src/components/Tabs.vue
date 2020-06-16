<template>
  <v-card>
    <v-tabs
      v-model="tab"
      centered
      color="black"
      grow
    >
      <v-tabs-slider></v-tabs-slider>
      <v-tab href="#tab-1">
        Описание
      </v-tab>

      <v-tab href="#tab-2">
        Характеристики
      </v-tab>
    </v-tabs>
    <v-tabs-items v-model="tab">
        <v-tab-item
        v-for="i in 2"
        :key="i"
        :value="'tab-' + i"
      >
        <v-card flat>
            <v-card-text v-if='i==1'>
                <p class='body-1 my-2'>
                    «Каждый ребенок — художник. Проблема в том, как сохранить это, несмотря на взросление». Эту фразу Пабло Пикассо создатели AP Collection считают своим девизом. Они пропагандирует ироничный взгляд на дизайн вещей, но при этом не теряя практичности.
                </p>
                <p class='body-1'>
                    История бренда началась с истории А (Алексиса) и P (Паулины). Тёплые отношения на расстоянии побудили их регулярно отправлять друг другу милые плюшевые игрушки, компенсирующие отсутствие объятий и нежности. Когда пара, наконец, встретилась и между ними возникла настоящая любовь, они решили создать общий дизайнерский проект. 
                </p>
                <p class='body-1'>
                    С 2015 года AP возвращают к жизни винтажную мебель, придавая ей свой неповторимый стиль. Каждый предмет уникален и создан вручную в Бельгии.
                </p>
                <p class='body-1'>
                    Кресло "Мисс Фламинго" подарит уникальность любому интерьеру. Птица фламинго - символ исполнения Ваших желаний.  
                </p>
            </v-card-text>
            <v-card-text v-else>
                <Characteristics/>
            </v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>

<script>
import Characteristics from './Characteristics'
export default {
    name:'Tabs',
    components: {
    Characteristics
    },
    data () {
        return {
            tab: null,
        }
    },
}
</script>
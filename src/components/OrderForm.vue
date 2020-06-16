<template>
  <v-form v-model="valid">
    <v-container class='pb-4 pt-1'>
      <v-row>
        <v-col cols="12" md="6" >
          <v-text-field
            v-model="firstname"
            label="Имя"
            required
            color="black"
          ></v-text-field>
        </v-col>

        <v-col cols="12" md="6" >
          <v-text-field
            v-model="phone"
            label="Номер телефона"
            required
            color="black"
          ></v-text-field>
        </v-col>
      </v-row>
      <v-btn block color="secondary" dark>Заказать</v-btn>
    </v-container>
  </v-form>
</template>

<script>
  export default {
    name: 'OrderForm',
    data: () => ({
      valid: false,
      firstname: '',
      phone: '',
    }),
  }
</script>
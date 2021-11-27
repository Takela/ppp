<template>
  <v-data-table dark
    :headers="headers"
    :items="desserts"
    :items-per-page="5"
    item-key="name"
    class="elevation-1"
    :footer-props="{
      showFirstLastPage: true,
      firstIcon: 'mdi-arrow-collapse-left',
      lastIcon: 'mdi-arrow-collapse-right',
      prevIcon: 'mdi-minus',
      nextIcon: 'mdi-plus'
    }"
  ></v-data-table>
</template>

<script>
  export default {
    data () {
      return {
        headers: [
          {
            text: '№',
            align: 'align-content',
            value: 'number',
          },
          { text: 'Действие',value: 'name', },

          {
            text: 'Время',value: 'gregori',
          }
        ],
        desserts: [
          {
            number: '1',
            name: 'проснутся',
            gregori: '9:00',
          },
          {
            number: '2',
            name: 'Умыться',
            gregori: '9:10',
          },
          {
            number: '3',
            name: 'Покушать или попить чай',
            gregori: '12:00-12:30',
          },
          {
            number: '4',
            name: 'школа',
            gregori: '12:40-19:00',
          },
          {
            number: '5',
            name: 'Дота?',
            gregori: '20:00-02:00',
          },
          
        ],
      }
    },
  }
</script>


<style>

</style>
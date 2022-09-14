<template>
  <div class='w-screen h-screen bg-gray-800 text-center flex flex-col items-center justify-center text-white'>
    <CustomTitle title='Vue CLI' />
    <CustomTable tableColor="green" :showBorder="true" :content="array1" />
    <CustomTable tableColor="blue" :showBorder="true" :content="array2" />
    <CustomTable tableColor="red" :showBorder="false" :content="array3" />
  </div>
</template>
<!------------------------------------------------------------------------------------------->
<script>

import CustomTable from './components/CustomTable.vue'
import CustomTitle from './components/CustomTitle.vue'
import '@/assets/tailwind.css'

export default {
  name: 'App',
  components: {
    CustomTable,
    CustomTitle
},
  data() {
    return {
      array1: [
        {
          bg: 'bg-transparent',
          list: ['Ciruela', '$143', '63']
        },
        {
          bg: 'bg-transparent',
          list: ['Manzana ', '$89', '43']
        },
        {
          bg: 'bg-transparent',
          list: ['Pera', '$54', '76']
        }
      ],
      array2: [
        {
          bg: 'bg-transparent',
          list: ['Apio', '$43', '123']
        },
        {
          bg: 'bg-transparent',
          list: ['Cebolla', '$25', '54']
        },
        {
          bg: 'bg-transparent',
          list: ['Esparrago', '$28', '79']
        }
      ],
      array3: [
        {
          bg: 'bg-transparent',
          list: ['Zapallo', '$43', '123']
        },
        {
          bg: 'bg-transparent',
          list: ['Calabaza', '$25', '54']
        },
        {
          bg: 'bg-black',
          list: ['Rabanito', '$28', '79']
        }
      ]
    }
  }
}
</script>
<!------------------------------------------------------------------------------------------->
<style>

</style>
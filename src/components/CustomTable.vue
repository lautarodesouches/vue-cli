<template>
  <div class='my-4 w-1/4' >
    <table class="table-auto rounded min-w-full" :class="'bg-'+ tableColor + '-500'">
      <thead :class="showBorder && 'border-b border-white'">
        <tr>
          <th>Nombre</th>
          <th>Precio</th>
          <th>Cantidad</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="item in content" :class="item.bg" :key="item">
          <td v-for="item in item.list" :key="item">
            {{item}}
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>
<!------------------------------------------------------------------------------------------->
<script>
export default {
  name: 'CustomTable',
  props: {
    tableColor: String,
    showBorder: Boolean,
    content: Array
  }
}
</script>
<!------------------------------------------------------------------------------------------->
<style scoped>

</style>
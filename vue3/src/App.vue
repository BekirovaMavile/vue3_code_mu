<script>
export default{
data(){
  return{
    products: [
      {
        id: 1,
        name: 'Alec Lightwood',
      },
      {
        id: 2,
        name: 'Isabel Lightwood',
      },
      {
        id: 3,
        name: 'Max Lightwood',
      },
    ]
  }
},
methods: {

}
}
</script>

<template>
  <p class="hunter" v-for="prod in products" :key='products.id'>{{ prod.name }}</p>
</template>

<style scoped>

</style>

<script>
export default{
data(){
  return{
    sity: 'Симферополь',
  }
},
methods: {

}
}
</script>

<template>
  <p class="hunter">В каком городе вы живете?</p>
    <select class="hunter" v-model="sity">
      <option>Симферополь</option>
      <option>Севастополь</option>
      <option>Ялта</option>
    </select>
    <p>{{ sity }}</p>
</template>

<style scoped>

</style>

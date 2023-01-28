<script>
export default{
data(){
  return{
    arr: ['Alec', 'Isabel', 'Max'],
  }
},
methods: {

}
}
</script>

<template>
  <ul class="hunter" v-for="(elem, key) in arr"> {{ key }} {{ elem }}</ul>
</template>

<style scoped>

</style>

<script>
export default{
data(){
  return{
    hidden: true,
    hidden1: false,
  }
},
}
</script>

<template>
<p class="hunter" v-if="hidden">Alec</p>
<p class="hunter" v-if="!hidden1">Lightwood</p>

</template>

<style scoped>

</style>

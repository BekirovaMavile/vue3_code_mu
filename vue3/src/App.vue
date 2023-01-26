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
<p v-if="hidden">text</p>
<p v-if="!hidden1">text</p>

</template>

<style scoped>

</style>

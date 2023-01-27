<script>
export default{
data(){
  return{
    visible: true,
    visible1: false,
  }
},
}
</script>

<template>
<p class="hunter" v-if="visible">text</p>
<p class="hunter" v-if="!visible1">text</p>

</template>

<style scoped>

</style>

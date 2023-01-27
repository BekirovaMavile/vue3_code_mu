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
<p class="hunter" v-if="visible">Alec</p>
<p class="hunter" v-if="!visible1">Lightwood</p>

</template>

<style scoped>

</style>

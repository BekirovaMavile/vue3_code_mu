<script>
export default{
data(){
  return{
    isHunter: true,
  }
},
methods: {

}
}
</script>

<template>
<p class="hunter" v-if="isHunter">Alec Lightwood</p>
<p class="hunter" v-else>Magnus Bane</p>
</template>

<style scoped>

</style>

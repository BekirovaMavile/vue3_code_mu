<script>
export default{
data(){
  return{
    isAdmin: true,
  }
},
methods: {

}
}
</script>

<template>
<p v-if="isAdmin">Hey!!!</p>
<p v-else>Admin false</p>
</template>

<style scoped>

</style>

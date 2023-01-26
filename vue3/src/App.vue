<script>
export default{
data(){
  return{
    hidden: true,
  }
},
methods: {
hide: function(){
  this.hidden = false;
}
}
}
</script>

<template>
  <button @click="hide">hide</button>
  <div v-if="hidden">
  <p>+++</p>
  <p>+++</p>
  <p>+++</p>
  </div>
</template>

<style scoped>

</style>

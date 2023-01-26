<script>
export default{
data(){
  return{
    text: 'one hargreaves',
  }
},
methods: {
  change: function(){
    this.text = 'five hargreaves';
},
change2: function(){
  this.text = 'two hargreaves'
}
}
}
</script>

<template>
<p>{{ text }}</p>
<button @click="change">text1</button>
<button @click="change2">text2</button>
</template>

<style scoped>

</style>

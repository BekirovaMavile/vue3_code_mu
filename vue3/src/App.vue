<script>
export default{
data(){
  return{
    hunter: ' ',
    conclave: ' ',
  }
},
methods: {
list: function(){

  }
}
}
</script>

<template>
<textarea class="text-field__input" v-model="hunter"></textarea>
<p class="hunter">{{ hunter }}</p>
<br>
<textarea class="text-field__input" v-model="conclave"></textarea>
<button class="button" @click="list">lists</button>
</template>

<style scoped>

</style>

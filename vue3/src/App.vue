<script>
export default{
data(){
  return{
    hunter: ' ',
    // conclave: ' ',
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
<button class="button" @click="list">lists</button>
<ul>
  <li v-for="hunt in hunter">{{ hunt }}</li>
</ul>
</template>

<style scoped>

</style>

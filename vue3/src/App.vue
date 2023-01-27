<script>
export default{
data(){
  return{
    cost: '120',
    amount: '5',
  }
},
computed: {
  price: function(){
    return this.cost *  this.amount;
  }
},
methods: {
change: function(){
  this.cost = '150'
}
}
}
</script>

<template>
<p class="hunter">{{ cost }}</p>
<p class="hunter">{{ amount }}</p>
<p class="hunter">{{ price }}</p>
<button class="button" @click="change">cost</button>
</template>

<style scoped>

</style>

<script>
export default{
data(){
  return{
    newHunter: '',
    hunters: ['Alec', 'Clary', 'Max', 'Isabel', 'Helen'],
  }
},
methods: {
  addHunter: function () {
    this.hunters.unshift(this.newHunter);
  }
}
}
</script>

<template>
<ul>
  <li v-for="(hunter, index) in 
			hunters" :key="index">
    {{ hunter }}
  </li>
</ul>
<input v-model="newHunter">
<button @click="addHunter">add</button>
</template>

<style scoped>

</style>

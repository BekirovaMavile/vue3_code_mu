<script>
export default{
data(){
  return{
    newHunter: '',
    hunters: ['Alec', 'Clary', 'Max', 'Isabel', 'Helen'],
  }
},
methods: {
  removeHunter: function (index) {
    this.hunters.splice(index, 1);
  }
}
}
</script>

<template>
<ul class="styled">
  <li v-for="(hunter, index) in 
			hunters" :key="index">
    {{ hunter }}
    <br>
    <button class="button" @click="removeHunter(index)">remove</button>
  </li>
</ul>
</template>

<style scoped>

</style>

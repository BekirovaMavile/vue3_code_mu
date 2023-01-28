<script>
export default{
data(){
  return{
    hunters: ['Alec', 'Isabel', 'Max'],
  }
},
methods: {
add: function(){
  this.hunters.push('Jace');
},
del: function(){
  this.hunters.shift();
},
del1: function () {
  this.hunters.pop();
},
splice: function(){
  this.hunters.splice(2, 1);
},
sort: function(){
  this.hunters.sort();
},
  reverse: function () {
    this.hunters.reverse();
  },
}
}
</script>

<template>
<ul class="styled">
  <li v-for="elem in hunters">{{ elem }}</li>
</ul>
<button class="button" @click="add">add hunter</button>
<br>
<button class="button" @click="del">delete hunter</button>
<br>
<button class="button" @click="del1">delete hunter at the end</button>
<br>
<button class="button" @click="splice">delete the penultimate hunter</button>
<br>
<button class="button" @click="sort">sort array</button>
<br>
<button class="button" @click="reverse">array in reverse order</button>
</template>

<style scoped>

</style>

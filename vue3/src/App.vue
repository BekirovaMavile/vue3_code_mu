<script>
export default{
data(){
  return{
    hunters: [
      {
        id: 1,
        name: 'Alec Lightwood',
        salary: 100,
        age: 19,
      },
      {
        id: 2,
        name: 'Jace Herondale',
        salary: 200,
        age: 18,
      },
      {
        id: 3,
        name: 'Magnus Bane',
        salary: 300,
        age: 25,
      },
    ],
  }
},
methods: {
  removeHunter: function (id) {
    this.hunters = this.hunters.filter((hunter) => {
      return hunter.id !== id;
    })
  }
}
}
</script>

<template>
<table class="hunter">
  <tr v-for="hunter in hunters" :key="hunter.id"> {{ hunter.name }} {{ hunter.salary }} {{ hunter.age }} <button class="button" @click="removeHunter(hunters.id)">remove</button>
</tr>
</table>
</template>

<style scoped>

</style>

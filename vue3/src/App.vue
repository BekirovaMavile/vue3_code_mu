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
    ]
  }
},
methods: {
  edit(hunter) {
    hunter.isEdit = true;
  },
  save(hunter) {
    hunter.isEdit = false;
  },
}
}
</script>

<template>
  <!-- <ul>
    <li v-for="user in users" :key="user.id">
<template v-if="!user.isEdit">
  {{ user.name }}
  {{ user.surn }}
  <button @click="edit(user)">
    edit
  </button>
</template>
<template v-else>
  <input v-model="user.name">
  <input v-model="user.surn">
  <button @click="save(user)">
    save
  </button>
</template>
    </li>
  </ul> -->
<table class="hunter">
<tr v-for="hunter in hunters" :key="hunter.id"> 
<template v-if="!hunter.isEdit">
  {{ hunter.name }} {{ hunter.salary }} {{ hunter.age }}<button class="button" @click="edit(hunter)">edit</button>
</template>
<template v-else>
  <input v-model="hunter.name">
  <input v-model="hunter.salary">
  <input v-model="hunter.age">
  <button class="button" @click="save(hunter)">
      save
  </button>
</template>
</tr>
</table>
</template>

<style scoped>

</style>

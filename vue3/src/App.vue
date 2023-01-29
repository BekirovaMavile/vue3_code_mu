<script>
import Hunter from './components/Employee.vue'

export default {
  data() {
    return {
      hunters: [
        {
          id: 1,
          name: 'Alec',
          salary: 1000,
          age: 19
        },
        {
          id: 2,
          name: 'Jace',
          salary: 1000,
          age: 18
        },
        {
          id: 3,
          name: 'Magnus',
          salary: 3000,
          age: 25
        },
      ],
    }
  },
  components: {
    Hunter
  }
}

</script>

<template>
<Hunter v-for="hunter in hunters" :name="hunter.name" :salary="hunter.salary" :age="hunter.age" :key="hunter.id" />
</template>


<style scoped>

</style>

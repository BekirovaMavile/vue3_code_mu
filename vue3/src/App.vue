<script>
import Hunter from './components/Employee.vue'

export default {
  data() {
    return {
      name: 'Alec Lightwood',
      salary: '1000',
      age: '19',
    }
  },
  components: {
    Hunter
  }
}

</script>

<template>
<Hunter :name="name" :salary="salary" :age="age"/>
</template>


<style scoped>

</style>

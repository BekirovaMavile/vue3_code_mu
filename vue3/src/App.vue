<script>
import Hunter from './components/Employee.vue'


export default {
  data() {
    return {
      
    }
  },
  components: {
    Hunter
  },
  methods: {
    hunterName(name) {
      console.log(name);
    },
    hunterSalary(name, salary){
console.log(name, salary);
    }
  }
}

</script>

<template>
<Hunter @show="hunterName" @show1="hunterSalary"/>
</template>


<style scoped>

</style>

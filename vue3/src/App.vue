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
  }
}

</script>

<template>
<Hunter @show="hunterName"/>
</template>


<style scoped>

</style>

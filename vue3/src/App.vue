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
    lightwood() {
      alert('Alec, Isabel, Gideon, Gabriel');
    },
    herondale(){
      alert('Jace, Will, Tessa, Lucy')
    }
  }
}

</script>

<template>
<Hunter @show="lightwood" @show1="herondale" />
</template>


<style scoped>

</style>

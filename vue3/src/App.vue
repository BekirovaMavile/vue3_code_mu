<script>
import Hunter from './components/Employee.vue'

export default {
  components: {
    Hunter
  }
}
</script>

<template>
<Hunter :name="['Alec', 'Clary', 'Jace', 'Isabel', 'Magnus', 'Rafael']"/>
</template>


<style scoped>

</style>

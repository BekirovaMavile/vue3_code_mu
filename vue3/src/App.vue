<script>
import Hunter from './components/Employee.vue'
import HunterForm from './components/HunterForm.vue'


export default {
  data() {
    return {
      hunters: [
        {
          id: 1,
          name: 'Alec',
          surn: 'Lightwood'
        },
        {
          id: 2,
          name: 'Jace',
          surn: 'Herondale'
        },
        {
          id: 3,
          name: 'Isabel',
          surn: 'Lightwood'
        },
      ],

    }
  },
  components: {
    Hunter, HunterForm
  },
  methods: {
    add(name, surn){
      let id = this.hunters.length + 1;
      this.hunters.push({
        id, name, surn
      });
    }
  }
}

</script>

<template>
<HunterForm @add="add"/>
</template>


<style scoped>

</style>

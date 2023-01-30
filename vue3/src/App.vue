<script>
import Hunter from './components/Employee.vue'


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
    Hunter
  },
  methods: {
    change(id, name, surn){
      this.hunters = this.hunters.map((hunter) => {
        if(hunter.id === id){
          hunter.name = name;
          hunter.surn = surn;
        }
        return hunter;
      });
    }
  }
}

</script>

<template>
<Hunter v-for   ="hunter in hunters"
		:id     ="hunter.id"
		:name   ="hunter.name"
		:surn   ="hunter.surn"
		:key    ="hunter.id"
    @change="change"/>
</template>


<style scoped>

</style>

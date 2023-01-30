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
    remove(id) {
      this.hunters = this.hunters.filter((hunter) => {
        return hunter.id !== id;
      })
    }
  }
}

</script>

<template>
<Hunter v-for   ="hunter in hunters"
		:id     ="hunter.id"
		:name   ="hunter.name"
		:surn   ="hunter.surn"
		@remove ="remove"
		:key    ="hunter.id"/>
</template>


<style scoped>

</style>

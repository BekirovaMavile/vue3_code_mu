<script>
export default{
data(){
  return{
    visible: true,
    visible1: true,
    visible2: true,
  }
},
methods: {
  toggle: function(){
    this.visible = !this.visible;
  },
  toggle1: function () {
    this.visible1 = !this.visible1;
  },
  toggle2: function () {
    this.visible2 = !this.visible2;
  }
}
}
</script>

<template>
<button @click="toggle">toggle</button>
{{visible ? 'hide' : 'show'}}
<button @click="toggle1">toggle</button>
{{visible1 ? 'hey' : 'bye'}}
<button @click="toggle2">toggle</button>
{{visible2 ? 'yes' : 'no'}}
</template>

<style scoped>

</style>

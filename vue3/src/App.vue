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
<button class="button" @click="toggle">toggle</button>
<p class="hunter">{{visible ? 'Alec' : 'Lightwood'}}</p>
<button class="button" @click="toggle1">toggle</button>
<p class="hunter">{{visible1 ? 'Magnus' : 'Bane'}}</p>
<button class="button" @click="toggle2">toggle</button>
<p class="hunter">{{visible2 ? 'Jace' : 'Herondale'}}</p>
</template>

<style scoped>

</style>

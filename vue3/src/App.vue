<script>
export default{
data(){
  return{
    checked: true,
    visible: true,
  }
},
methods: {
  toggle: function () {
    this.checked = false;
    this.visible = !this.visible;
  },
}
}
</script>

<template>
<input class="text-field__input" type="checkbox" v-model="checked"> 
<button class="button" @click="toggle">toggle</button>
<p class="hunter" v-if="visible">{{ checked ? 'Alec' : 'Jace' }}</p>
</template>

<style scoped>

</style>

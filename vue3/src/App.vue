<script>
export default{
data(){
  return{
    visible: true,
    visible2: true,
    visible3: true,
  }
},
methods: {
  toggle: function(){
    this.visible = !this.visible;
  },
  toggle2: function () {
    this.visible2 = !this.visible2;
  },
  toggle3: function () {
    this.visible3 = !this.visible3;
  }
}
}
</script>

<template>
<button class="button" @click="toggle">toggle</button>
<p class="hunter" v-if="visible">Alec</p>
<button class="button" @click="toggle2">toggle</button>
<p class="hunter" v-if="visible2">Isabel</p>
<button class="button" @click="toggle3">toggle</button>
<p class="hunter" v-if="visible3">Magnus</p>
</template>

<style scoped>

</style>

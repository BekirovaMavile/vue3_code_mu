<script>
export default{
data(){
  return{
    visible: true,
btnHide: true,
btnVis: false,
  }
},
methods: {
  hide: function(){
    this.visible = false;
    this.btnHide = false;
    this.btnVis = true;
  },
  vis: function(){
    this.visible = true;
    this.btnHide = true;
    this.btnVis = false;
  }
}
}
</script>

<template>
<button @click="hide" v-if="btnHide">hide</button>
<button @click="vis" v-if="btnVis">visible</button>
<p v-if="visible">text</p>
</template>

<style scoped>

</style>

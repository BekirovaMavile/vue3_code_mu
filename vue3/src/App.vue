<script>
export default{
data(){
  return{
    styles: {
      hidden: true,
    },
  }
},
methods: {
setDone:function(){
  this.styles.hidden = false;
}
}
}
</script>

<template>
<p class="hunter">Shadowhunter</p>
<p :class="styles">Conclave</p>
<button @click="setDone">hide</button>
</template>

<style scoped>
p.hidden{
  display: none;
}
</style>

<script>
export default{
data(){
  
},
methods: {
  show: function(){
    alert(new Date().toLocaleDateString());
  }
}
}
</script>

<template>
<button class="button" v-on:mouseover="show">mouse</button>
<button class="button" @click="show">click</button>
</template>

<style scoped>

</style>

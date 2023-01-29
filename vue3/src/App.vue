<script>
export default{
data(){
  return{
  hunter: ' ',
  hunters: ' '
  }
},
methods: {
  // vm.submit()
}
}
</script>

<template>
<input class="text-field__input" v-model="hunter" v-on:keyup.enter="submit">
<p>{{ hunter }}</p>
<br>
<a href="#" class="inline-link-1" v-on:keyup.ctrl="sub">Conclave</a>
<p ></p>
</template>

<style scoped>

</style>

<script>
export default{
data(){
  return{
    obj: {
      done: true,
      selected: false,
    },
  }
},
methods: {

}
}
</script>

<template>
<p :class="selected">Shadowhunter</p>
<p :class="obj">Conclave</p>
</template>

<style scoped>
.selected{
  padding: 10px;
    margin: 10px;
    background: #08C;
    color: white;
    font-weight: bold;
    text-decoration: none;
}
.done {
  padding: 10px;
  margin: 10px;
  background: #08C;
  color: white;
  font-weight: bold;
  text-decoration: none;
}
</style>

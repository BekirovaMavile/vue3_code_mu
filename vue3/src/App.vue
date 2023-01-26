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
<a href="https://www.google.ru/" onclick="event.preventDefault()">Link</a>
<br>
<br>
<button @click.once="show">click</button>
</template>

<style scoped>

</style>

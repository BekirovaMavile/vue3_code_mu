<script>
export default{
data(){
  return{
    cssClass: 'hunt night',
  }
},
methods: {

}
}
</script>

<template>
<p :class="cssClass">Shadowhunter</p>
</template>

<style scoped>
.hunt{
  padding: 10px;
    margin: 10px;
    background: #08C;
    color: white;
    font-weight: bold;
    text-decoration: none;
}
</style>

<script>
export default{
data(){
  return{
    day: 'Пятница',
  }
},
methods: {

}
}
</script>

<template>
<p class="hunter" v-if="day === 'Понедельник'">Понедельник</p>
<p class="hunter" v-if="day === 'Вторник'">Вторник</p>
<p class="hunter" v-if="day === 'Среда'">Среда</p>
<p class="hunter" v-if="day === 'Четверг'">Четверг</p>
<p class="hunter" v-if="day === 'Пятница'">Пятница</p>
<p class="hunter" v-if="day === 'Суббота'">Суббота</p>
<p class="hunter" v-if="day === 'Воскресенье'">Воскресенье</p>
</template>

<style scoped>

</style>

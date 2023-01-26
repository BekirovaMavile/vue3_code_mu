<script>
export default{
data(){
  return{
    date: '1'
  }
},
methods: {
  show: function(){
    let date = this.cape(this.date);
    alert( WeekDay(date));
  },
  cape: function WeekDay(date){
    let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
    return days[date.getDay()];
  }
}
}
</script>

<template>
<button v-on:mouseover="show">mouse</button>
<button @click="show">click</button>
</template>

<style scoped>
/* header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
} */
</style>

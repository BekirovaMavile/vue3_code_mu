<script>
export default{
data(){
  return{
    language: '',
  }
},
methods: {

}
}
</script>

<template>
  <div class="hunter">
    <p>Какой язык ваш родной?</p>
<input name="radio" type="radio" v-model="language" value="Крымскотатарский">
<label for="">Крымскотатарский</label>
<br>
<input name="radio" type="radio" v-model="language" value="Русский">
<label for="">Русский</label>
<br>
<input name="radio" type="radio" v-model="language" value="Испанский">
<label for="">Испанский</label>
</div>
<!-- <p v-if="value === 'Крымскотатарский'">Хош кельдинъиз</p>
<p v-else-if="value === 'Русский'">Добро пожаловать</p>
<p v-else-if="value === 'Испанский'">Bienvenido</p>
<p v-else=''> </p> -->

<p>Ваш выбор: {{ language }}</p>
<br>
</template>

<style scoped>

</style>

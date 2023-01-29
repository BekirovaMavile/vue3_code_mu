<script>
export default {
    props: ['name'],
    data() {
        return {

        }
    }
}
</script>

<template>
<ul class="styled">
    <li v-for="hunter in name">{{ hunter }}</li>
</ul>
</template>